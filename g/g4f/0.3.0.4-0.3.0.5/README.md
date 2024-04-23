# Comparing `tmp/g4f-0.3.0.4.tar.gz` & `tmp/g4f-0.3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.4.tar", last modified: Mon Apr 22 01:19:38 2024, max compression
+gzip compressed data, was "g4f-0.3.0.5.tar", last modified: Mon Apr 22 18:08:36 2024, max compression
```

## Comparing `g4f-0.3.0.4.tar` & `g4f-0.3.0.5.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.242879 g4f-0.3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-22 01:19:34.000000 g4f-0.3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 01:19:34.000000 g4f-0.3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-04-22 01:19:38.242879 g4f-0.3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-22 01:19:34.000000 g4f-0.3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.202880 g4f-0.3.0.4/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.210879 g4f-0.3.0.4/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21313 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.214879 g4f-0.3.0.4/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.218879 g4f-0.3.0.4/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.218879 g4f-0.3.0.4/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.222879 g4f-0.3.0.4/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.222879 g4f-0.3.0.4/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.226879 g4f-0.3.0.4/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.230879 g4f-0.3.0.4/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.230879 g4f-0.3.0.4/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.230879 g4f-0.3.0.4/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.230879 g4f-0.3.0.4/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.198880 g4f-0.3.0.4/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.230879 g4f-0.3.0.4/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.234879 g4f-0.3.0.4/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.234879 g4f-0.3.0.4/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45952 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.234879 g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.234879 g4f-0.3.0.4/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.238879 g4f-0.3.0.4/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.238879 g4f-0.3.0.4/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.238879 g4f-0.3.0.4/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.238879 g4f-0.3.0.4/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-22 01:19:34.000000 g4f-0.3.0.4/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:19:38.238879 g4f-0.3.0.4/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 01:19:38.000000 g4f-0.3.0.4/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:19:38.242879 g4f-0.3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-22 01:19:34.000000 g4f-0.3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.815373 g4f-0.3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-22 18:08:32.000000 g4f-0.3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 18:08:32.000000 g4f-0.3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    53884 2024-04-22 18:08:36.815373 g4f-0.3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    50688 2024-04-22 18:08:32.000000 g4f-0.3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.775373 g4f-0.3.0.5/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.783373 g4f-0.3.0.5/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21313 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.787373 g4f-0.3.0.5/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.791373 g4f-0.3.0.5/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.791373 g4f-0.3.0.5/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.795373 g4f-0.3.0.5/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.795373 g4f-0.3.0.5/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.795373 g4f-0.3.0.5/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.799373 g4f-0.3.0.5/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.771373 g4f-0.3.0.5/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.803373 g4f-0.3.0.5/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.807373 g4f-0.3.0.5/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45952 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.807373 g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.807373 g4f-0.3.0.5/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.807373 g4f-0.3.0.5/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.811373 g4f-0.3.0.5/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.811373 g4f-0.3.0.5/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.811373 g4f-0.3.0.5/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-22 18:08:32.000000 g4f-0.3.0.5/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:08:36.811373 g4f-0.3.0.5/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    53884 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 18:08:36.000000 g4f-0.3.0.5/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:08:36.815373 g4f-0.3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-22 18:08:32.000000 g4f-0.3.0.5/setup.py
```

### Comparing `g4f-0.3.0.4/LICENSE` & `g4f-0.3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/PKG-INFO` & `g4f-0.3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.4
+Version: 0.3.0.5
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -478,19 +478,20 @@
 | openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://huggingface.co/) |
 | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https://inflection.ai/) |
 
 ### Image and Vision Models
 
 | Label | Provider | Image Model | Vision Model | Website |
 | ----- | -------- | ----------- | ------------ | ------- |
-| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-4-vision | [bing.com](https://bing.com/chat) |
+| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | gemini| gemini | [gemini.google.com](https://gemini.google.com) |
+| Gemini API | `g4f.Provider.GeminiPro` | ❌| gemini-1.5-pro-latest | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | meta| ❌ | [meta.ai](https://www.meta.ai) |
-| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| ❌ | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) |
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.4 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.5 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -368,25 +368,26 @@
 lzlv_70b_fp16_hf | Huggingface | g4f.Provider.DeepInfra | [huggingface.co]
 (https://huggingface.co/) | | airoboros-70b | Huggingface |
 g4f.Provider.DeepInfra | [huggingface.co](https://huggingface.co/) | |
 openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://
 huggingface.co/) | | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https:
 //inflection.ai/) | ### Image and Vision Models | Label | Provider | Image
 Model | Vision Model | Website | | ----- | -------- | ----------- | -----------
-- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-
-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
+- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 |
+gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com]
 (https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` | gemini| gemini |
-[gemini.google.com](https://gemini.google.com) | | Meta AI |
-`g4f.Provider.MetaAI` | meta| â | [meta.ai](https://www.meta.ai) | | OpenAI
-ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com]
-(https://chat.openai.com) | | Replicate | `g4f.Provider.Replicate` | stability-
-ai/sdxl| â | [replicate.com](https://replicate.com) | | You.com |
-`g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) | ## ð
-Powered by gpt4free
+[gemini.google.com](https://gemini.google.com) | | Gemini API |
+`g4f.Provider.GeminiPro` | â| gemini-1.5-pro-latest | [ai.google.dev](https:/
+/ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | meta| â | [meta.ai]
+(https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
+`g4f.Provider.Replicate` | stability-ai/sdxl| â | [replicate.com](https://
+replicate.com) | | You.com | `g4f.Provider.You` | dall-e| agent | [you.com]
+(https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.0.4/README.md` & `g4f-0.3.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -400,19 +400,20 @@
 | openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://huggingface.co/) |
 | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https://inflection.ai/) |
 
 ### Image and Vision Models
 
 | Label | Provider | Image Model | Vision Model | Website |
 | ----- | -------- | ----------- | ------------ | ------- |
-| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-4-vision | [bing.com](https://bing.com/chat) |
+| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | gemini| gemini | [gemini.google.com](https://gemini.google.com) |
+| Gemini API | `g4f.Provider.GeminiPro` | ❌| gemini-1.5-pro-latest | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | meta| ❌ | [meta.ai](https://www.meta.ai) |
-| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| ❌ | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) |
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
```

#### html2text {}

```diff
@@ -326,25 +326,26 @@
 lzlv_70b_fp16_hf | Huggingface | g4f.Provider.DeepInfra | [huggingface.co]
 (https://huggingface.co/) | | airoboros-70b | Huggingface |
 g4f.Provider.DeepInfra | [huggingface.co](https://huggingface.co/) | |
 openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://
 huggingface.co/) | | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https:
 //inflection.ai/) | ### Image and Vision Models | Label | Provider | Image
 Model | Vision Model | Website | | ----- | -------- | ----------- | -----------
-- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-
-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
+- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 |
+gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com]
 (https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` | gemini| gemini |
-[gemini.google.com](https://gemini.google.com) | | Meta AI |
-`g4f.Provider.MetaAI` | meta| â | [meta.ai](https://www.meta.ai) | | OpenAI
-ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com]
-(https://chat.openai.com) | | Replicate | `g4f.Provider.Replicate` | stability-
-ai/sdxl| â | [replicate.com](https://replicate.com) | | You.com |
-`g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) | ## ð
-Powered by gpt4free
+[gemini.google.com](https://gemini.google.com) | | Gemini API |
+`g4f.Provider.GeminiPro` | â| gemini-1.5-pro-latest | [ai.google.dev](https:/
+/ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | meta| â | [meta.ai]
+(https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
+`g4f.Provider.Replicate` | stability-ai/sdxl| â | [replicate.com](https://
+replicate.com) | | You.com | `g4f.Provider.You` | dall-e| agent | [you.com]
+(https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.0.4/g4f/Provider/Aichatos.py` & `g4f-0.3.0.5/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Aura.py` & `g4f-0.3.0.5/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Bing.py` & `g4f-0.3.0.5/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.5/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Blackbox.py` & `g4f-0.3.0.5/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.5/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.5/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.5/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.5/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.5/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.5/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Cnote.py` & `g4f-0.3.0.5/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Cohere.py` & `g4f-0.3.0.5/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.5/g4f/Provider/DeepInfra.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from ..image import to_data_uri
 from .needs_auth.Openai import Openai
 
 class DeepInfra(Openai):
     label = "DeepInfra"
     url = "https://deepinfra.com"
     working = True
+    needs_auth = False
     has_auth = True
     supports_stream = True
     supports_message_history = True
     default_model = "meta-llama/Meta-Llama-3-70b-instruct"
     default_vision_model = "llava-hf/llava-1.5-7b-hf"
     model_aliases = {
-        'mixtral-8x22b': 'HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1'
+        'dbrx-instruct': 'databricks/dbrx-instruct',
     }
 
     @classmethod
     def get_models(cls):
         if not cls.models:
             url = 'https://api.deepinfra.com/models/featured'
             models = requests.get(url).json()
```

### Comparing `g4f-0.3.0.4/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.5/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.5/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Ecosia.py` & `g4f-0.3.0.5/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Feedough.py` & `g4f-0.3.0.5/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.5/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.5/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.5/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.5/g4f/Provider/GeminiPro.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from ..typing import AsyncResult, Messages, ImageType
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from ..image import to_bytes, is_accepted_format
 from ..errors import MissingAuthError
 from .helper import get_connector
 
 class GeminiPro(AsyncGeneratorProvider, ProviderModelMixin):
+    label = "Gemini API"
     url = "https://ai.google.dev"
     working = True
     supports_message_history = True
     needs_auth = True
-    default_model = "gemini-pro"
-    models = ["gemini-pro", "gemini-pro-vision"]
+    default_model = "gemini-1.5-pro-latest"
+    default_vision_model = default_model
+    models = [default_model, "gemini-pro", "gemini-pro-vision"]
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         stream: bool = False,
@@ -28,19 +30,18 @@
         api_key: str = None,
         api_base: str = "https://generativelanguage.googleapis.com/v1beta",
         use_auth_header: bool = False,
         image: ImageType = None,
         connector: BaseConnector = None,
         **kwargs
     ) -> AsyncResult:
-        model = "gemini-pro-vision" if not model and image is not None else model
         model = cls.get_model(model)
 
         if not api_key:
-            raise MissingAuthError('Missing "api_key"')
+            raise MissingAuthError('Add a "api_key"')
 
         headers = params = None
         if use_auth_header:
             headers = {"Authorization": f"Bearer {api_key}"}
         else:
             params = {"key": api_key}
```

### Comparing `g4f-0.3.0.4/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.5/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/GigaChat.py` & `g4f-0.3.0.5/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.5/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.5/g4f/Provider/HuggingChat.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 
 import json
 import requests
 from aiohttp import ClientSession, BaseConnector
 
 from ..typing import AsyncResult, Messages
 from ..requests.raise_for_status import raise_for_status
+from ..providers.conversation import BaseConversation
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from .helper import format_prompt, get_connector
+from .helper import format_prompt, get_connector, get_cookies
 
 class HuggingChat(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://huggingface.co/chat"
     working = True
+    needs_auth = True
     default_model = "mistralai/Mixtral-8x7B-Instruct-v0.1"
     models = [
         "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
         'CohereForAI/c4ai-command-r-plus',
         'mistralai/Mixtral-8x7B-Instruct-v0.1',
         'google/gemma-1.1-7b-it',
         'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO',
         'mistralai/Mistral-7B-Instruct-v0.2',
         'meta-llama/Meta-Llama-3-70B-Instruct'
     ]
-    model_aliases = {
-        "openchat/openchat_3.5": "openchat/openchat-3.5-0106",
-    }
 
     @classmethod
     def get_models(cls):
         if not cls.models:
             url = f"{cls.url}/__data.json"
             data = requests.get(url).json()["nodes"][0]["data"]
             models = [data[key]["name"] for key in data[data[0]["models"]]]
@@ -41,42 +40,54 @@
         model: str,
         messages: Messages,
         stream: bool = True,
         proxy: str = None,
         connector: BaseConnector = None,
         web_search: bool = False,
         cookies: dict = None,
+        conversation: Conversation = None,
+        return_conversation: bool = False,
+        delete_conversation: bool = True,
         **kwargs
     ) -> AsyncResult:
         options = {"model": cls.get_model(model)}
+        if cookies is None:
+            cookies = get_cookies("huggingface.co", False)
+        if return_conversation:
+            delete_conversation = False
 
         system_prompt = "\n".join([message["content"] for message in messages if message["role"] == "system"])
         if system_prompt:
             options["preprompt"] = system_prompt
             messages = [message for message in messages if message["role"] != "system"]
         headers = {
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
         }
         async with ClientSession(
             cookies=cookies,
             headers=headers,
             connector=get_connector(connector, proxy)
         ) as session:
-            async with session.post(f"{cls.url}/conversation", json=options) as response:
-                await raise_for_status(response)
-                conversation_id = (await response.json())["conversationId"]
+            if conversation is None:
+                async with session.post(f"{cls.url}/conversation", json=options) as response:
+                    await raise_for_status(response)
+                    conversation_id = (await response.json())["conversationId"]
+                if return_conversation:
+                    yield Conversation(conversation_id)
+            else:
+                conversation_id = conversation.conversation_id
             async with session.get(f"{cls.url}/conversation/{conversation_id}/__data.json") as response:
                 await raise_for_status(response)
                 data: list = (await response.json())["nodes"][1]["data"]
                 keys: list[int] = data[data[0]["messages"]]
                 message_keys: dict = data[keys[0]]
                 message_id: str = data[message_keys["id"]]
             options = {
                 "id": message_id,
-                "inputs": format_prompt(messages),
+                "inputs": format_prompt(messages) if conversation is None else messages[-1]["content"],
                 "is_continue": False,
                 "is_retry": False,
                 "web_search": web_search
             }
             async with session.post(f"{cls.url}/conversation/{conversation_id}", json=options) as response:
                 first_token = True
                 async for line in response.content:
@@ -88,9 +99,14 @@
                         token = line["token"]
                         if first_token:
                             token = token.lstrip()
                             first_token = False
                         yield token
                     elif line["type"] == "finalAnswer":
                         break
-            async with session.delete(f"{cls.url}/conversation/{conversation_id}") as response:
-                await raise_for_status(response)
+            if delete_conversation:
+                async with session.delete(f"{cls.url}/conversation/{conversation_id}") as response:
+                    await raise_for_status(response)
+
+class Conversation(BaseConversation):
+    def __init__(self, conversation_id: str) -> None:
+        self.conversation_id = conversation_id
```

### Comparing `g4f-0.3.0.4/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.5/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Koala.py` & `g4f-0.3.0.5/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Liaobots.py` & `g4f-0.3.0.5/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Llama.py` & `g4f-0.3.0.5/g4f/Provider/Llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 
 
 class Llama(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://www.llama2.ai"
     working = True
     supports_message_history = True
-    default_model = "meta/llama-3-70b-chat"
+    default_model = "meta/meta-llama-3-70b-instruct"
     models = [
         "meta/llama-2-7b-chat",
         "meta/llama-2-13b-chat",
         "meta/llama-2-70b-chat",
         "meta/meta-llama-3-8b-instruct",
         "meta/meta-llama-3-70b-instruct",
     ]
     model_aliases = {
-        "meta-llama/Meta-Llama-3-8b-instruct": "meta/meta-llama-3-8b-instruct",
-        "meta-llama/Meta-Llama-3-70b-instruct": "meta/meta-llama-3-70b-instruct",
+        "meta-llama/Meta-Llama-3-8B-Instruct": "meta/meta-llama-3-8b-instruct",
+        "meta-llama/Meta-Llama-3-70B-Instruct": "meta/meta-llama-3-70b-instruct",
         "meta-llama/Llama-2-7b-chat-hf": "meta/llama-2-7b-chat",
         "meta-llama/Llama-2-13b-chat-hf": "meta/llama-2-13b-chat",
         "meta-llama/Llama-2-70b-chat-hf": "meta/llama-2-70b-chat",
     }
 
     @classmethod
     async def create_async_generator(
```

### Comparing `g4f-0.3.0.4/g4f/Provider/Local.py` & `g4f-0.3.0.5/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/MetaAI.py` & `g4f-0.3.0.5/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.0.5/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.5/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Pi.py` & `g4f-0.3.0.5/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Replicate.py` & `g4f-0.3.0.5/g4f/Provider/Replicate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from ..requests.aiohttp import StreamSession
 from ..errors import ResponseError, MissingAuthError
 
 class Replicate(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://replicate.com"
     working = True
     default_model = "meta/meta-llama-3-70b-instruct"
+    model_aliases = {
+        "meta-llama/Meta-Llama-3-70B-Instruct": default_model
+    }
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         api_key: str = None,
```

### Comparing `g4f-0.3.0.4/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.5/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/Vercel.py` & `g4f-0.3.0.5/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.5/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/You.py` & `g4f-0.3.0.5/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/__init__.py` & `g4f-0.3.0.5/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.5/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.5/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.5/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.5/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.5/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.5/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.5/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.5/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.5/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.5/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.5/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.5/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.5/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.5/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.5/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.5/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.5/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.5/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.5/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.5/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.5/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.5/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.5/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.5/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.5/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.5/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.5/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.5/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.5/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.5/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.5/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.5/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/Provider/you/har_file.py` & `g4f-0.3.0.5/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/__init__.py` & `g4f-0.3.0.5/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/api/__init__.py` & `g4f-0.3.0.5/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/api/_logging.py` & `g4f-0.3.0.5/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/cli.py` & `g4f-0.3.0.5/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/async_client.py` & `g4f-0.3.0.5/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/client.py` & `g4f-0.3.0.5/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/helper.py` & `g4f-0.3.0.5/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/image_models.py` & `g4f-0.3.0.5/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/service.py` & `g4f-0.3.0.5/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/stubs.py` & `g4f-0.3.0.5/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/client/types.py` & `g4f-0.3.0.5/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/cookies.py` & `g4f-0.3.0.5/g4f/cookies.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 from .typing import Dict, Cookies
 from .errors import MissingRequirementsError
 from . import debug
 
 # Global variable to store cookies
 _cookies: Dict[str, Cookies] = {}
 
+DOMAINS = [
+    ".bing.com",
+    ".meta.ai",
+    ".google.com",
+    "www.whiterabbitneo.com",
+    "huggingface.co"
+]
+
 if has_browser_cookie3 and os.environ.get('DBUS_SESSION_BUS_ADDRESS') == "/dev/null":
     _LinuxPasswordManager.get_password = lambda a, b: b"secret"
 
 def get_cookies(domain_name: str = '', raise_requirements_error: bool = True, single_browser: bool = False) -> Dict[str, str]:
     """
     Load cookies for a given domain from all supported browsers and cache the results.
 
@@ -84,14 +92,23 @@
             pass
         except Exception as e:
             if debug.logging:
                 print(f"Error reading cookies from {cookie_fn.__name__} for {domain_name}: {e}")
     return cookies
 
 def read_cookie_files(dirPath: str = "./har_and_cookies"):
+    def get_domain(v: dict) -> str:
+        host = [h["value"] for h in v['request']['headers'] if h["name"].lower() in ("host", ":authority")]
+        if not host:
+            return
+        host = host.pop()
+        for d in DOMAINS:
+            if d in host:
+                return d
+
     global _cookies
     harFiles = []
     cookieFiles = []
     for root, dirs, files in os.walk(dirPath):
         for file in files:
             if file.endswith(".har"):
                 harFiles.append(os.path.join(root, file))
@@ -105,22 +122,23 @@
             except json.JSONDecodeError:
                 # Error: not a HAR file!
                 continue
             if debug.logging:
                 print("Read .har file:", path)
             new_cookies = {}
             for v in harFile['log']['entries']:
+                domain = get_domain(v)
+                if domain is None:
+                    continue
                 v_cookies = {}
                 for c in v['request']['cookies']:
-                    if c['domain'] not in v_cookies:
-                        v_cookies[c['domain']] = {}
-                    v_cookies[c['domain']][c['name']] = c['value']
-                for domain, c in v_cookies.items():
-                    _cookies[domain] = c
-                    new_cookies[domain] = len(c)
+                    v_cookies[c['name']] = c['value']
+                if len(v_cookies) > 0:
+                    _cookies[domain] = v_cookies
+                    new_cookies[domain] = len(v_cookies)
             if debug.logging:
                 for domain, new_values in new_cookies.items():
                     print(f"Cookies added: {new_values} from {domain}")
     for path in cookieFiles:
         with open(path, 'rb') as file:
             try:
                 cookieFile = json.load(file)
```

### Comparing `g4f-0.3.0.4/g4f/errors.py` & `g4f-0.3.0.5/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/__init__.py` & `g4f-0.3.0.5/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/index.html` & `g4f-0.3.0.5/g4f/gui/client/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,15 @@
                 <textarea id="Bing-api_key" name="Bing[api_key]" class="BingCreateImages-api_key" placeholder="&quot;_U&quot; cookie"></textarea>
             </div>
             <div class="field box">
                 <label for="DeepInfra-api_key" class="label" title="">DeepInfra:</label>
                 <textarea id="DeepInfra-api_key" name="DeepInfra[api_key]" class="DeepInfraImage-api_key" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
-                <label for="Gemini-api_key" class="label" title="">Gemini:</label>
-                <textarea id="Gemini-api_key" name="Gemini[api_key]" placeholder="&quot;__Secure-1PSID&quot; cookie"></textarea>
-            </div>
-            <div class="field box">
-                <label for="GeminiPro-api_key" class="label" title="">GeminiPro API:</label>
+                <label for="GeminiPro-api_key" class="label" title="">Gemini API:</label>
                 <textarea id="GeminiPro-api_key" name="GeminiPro[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
                 <label for="Groq-api_key" class="label" title="">Groq:</label>
                 <textarea id="Groq-api_key" name="Groq[api_key]" placeholder="api_key"></textarea>
             </div>
             <div class="field box">
@@ -153,14 +149,18 @@
                 <label for="OpenaiAccount-api_key" class="label" title="">OpenAI ChatGPT:</label>
                 <textarea id="OpenaiAccount-api_key" name="OpenaiAccount[api_key]" placeholder="access_key"></textarea>
             </div>
             <div class="field box">
                 <label for="OpenRouter-api_key" class="label" title="">OpenRouter:</label>
                 <textarea id="OpenRouter-api_key" name="OpenRouter[api_key]" placeholder="api_key"></textarea>
             </div>
+            <div class="field box">
+                <label for="Replicate-api_key" class="label" title="">Replicate:</label>
+                <textarea id="Replicate-api_key" name="Replicate[api_key]" class="ReplicateImage-api_key" placeholder="api_key"></textarea>
+            </div>
             </div>
             <div class="bottom_buttons">
                 <button onclick="delete_conversations()">
                     <i class="fa-regular fa-trash"></i>
                     <span>Clear Conversations</span>
                 </button>
                 <button onclick="save_storage()">
```

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.5/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.5/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.5/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.5/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/api.py` & `g4f-0.3.0.5/g4f/gui/server/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,29 +41,41 @@
                 ]
             else:
                 return [];
 
     @staticmethod
     def get_image_models() -> list[dict]:
         image_models = []
+        index = []
         for provider in __providers__:
             if hasattr(provider, "image_models"):
                 if hasattr(provider, "get_models"):
                     provider.get_models()
                 parent = provider
                 if hasattr(provider, "parent"):
                     parent = __map__[provider.parent]
-                for model in provider.image_models:
-                    image_models.append({
-                        "provider": parent.__name__,
-                        "url": parent.url,
-                        "label": parent.label if hasattr(parent, "label") else None,
-                        "image_model": model,
-                        "vision_model": parent.default_vision_model if hasattr(parent, "default_vision_model") else None
-                    })
+                if parent.__name__ not in index:
+                    for model in provider.image_models:
+                        image_models.append({
+                            "provider": parent.__name__,
+                            "url": parent.url,
+                            "label": parent.label if hasattr(parent, "label") else None,
+                            "image_model": model,
+                            "vision_model": parent.default_vision_model if hasattr(parent, "default_vision_model") else None
+                        })
+                        index.append(parent.__name__)
+            elif hasattr(provider, "default_vision_model") and provider.__name__ not in index:
+                image_models.append({
+                    "provider": provider.__name__,
+                    "url": provider.url,
+                    "label": provider.label if hasattr(provider, "label") else None,
+                    "image_model": None,
+                    "vision_model": provider.default_vision_model
+                })
+                index.append(provider.__name__)
         return image_models
 
     @staticmethod
     def get_providers() -> list[str]:
         """
         Return a list of all working providers.
         """
```

### Comparing `g4f-0.3.0.4/g4f/gui/server/backend.py` & `g4f-0.3.0.5/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/config.py` & `g4f-0.3.0.5/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/internet.py` & `g4f-0.3.0.5/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/js_api.py` & `g4f-0.3.0.5/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/server/website.py` & `g4f-0.3.0.5/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/gui/webview.py` & `g4f-0.3.0.5/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/image.py` & `g4f-0.3.0.5/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/local/__init__.py` & `g4f-0.3.0.5/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/locals/models.py` & `g4f-0.3.0.5/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/locals/provider.py` & `g4f-0.3.0.5/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/models.py` & `g4f-0.3.0.5/g4f/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     HuggingChat,
     HuggingFace,
     Koala,
     Liaobots,
     Llama,
     OpenaiChat,
     PerplexityLabs,
+    Replicate,
     Pi,
     Vercel,
     You,
 )
 
 
 @dataclass(unsafe_hash=True)
@@ -133,27 +134,27 @@
     base_provider = 'meta',
     best_provider = RetryProvider([Llama, DeepInfra])
 )
 
 llama2_70b = Model(
     name          = "meta-llama/Llama-2-70b-chat-hf",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama, DeepInfra, HuggingChat])
+    best_provider = RetryProvider([Llama, DeepInfra])
 )
 
 llama3_8b_instruct = Model(
-    name          = "meta-llama/Meta-Llama-3-8b-instruct",
+    name          = "meta-llama/Meta-Llama-3-8B-Instruct",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama])
+    best_provider = RetryProvider([Llama, DeepInfra, Replicate])
 )
 
 llama3_70b_instruct = Model(
-    name          = "meta-llama/Meta-Llama-3-70b-instruct",
+    name          = "meta-llama/Meta-Llama-3-70B-Instruct",
     base_provider = "meta",
-    best_provider = RetryProvider([Llama, HuggingChat])
+    best_provider = RetryProvider([Llama, DeepInfra])
 )
 
 codellama_34b_instruct = Model(
     name          = "codellama/CodeLlama-34b-Instruct-hf",
     base_provider = "meta",
     best_provider = HuggingChat
 )
@@ -164,15 +165,15 @@
     best_provider = RetryProvider([DeepInfra, PerplexityLabs])
 )
 
 # Mistral
 mixtral_8x7b = Model(
     name          = "mistralai/Mixtral-8x7B-Instruct-v0.1",
     base_provider = "huggingface",
-    best_provider = RetryProvider([DeepInfra, HuggingChat, HuggingFace, PerplexityLabs])
+    best_provider = RetryProvider([DeepInfra, HuggingFace, PerplexityLabs])
 )
 
 mistral_7b = Model(
     name          = "mistralai/Mistral-7B-Instruct-v0.1",
     base_provider = "huggingface",
     best_provider = RetryProvider([HuggingChat, HuggingFace, PerplexityLabs])
 )
@@ -182,15 +183,15 @@
     base_provider = "huggingface",
     best_provider = DeepInfra
 )
 
 mixtral_8x22b = Model(
     name          = "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
     base_provider = "huggingface",
-    best_provider = RetryProvider([HuggingChat, DeepInfra])
+    best_provider = DeepInfra
 )
 
 # Misc models
 dolphin_mixtral_8x7b = Model(
     name          = "cognitivecomputations/dolphin-2.6-mixtral-8x7b",
     base_provider = "huggingface",
     best_provider = DeepInfra
@@ -207,15 +208,15 @@
     base_provider = "huggingface",
     best_provider = DeepInfra
 )
 
 openchat_35 = Model(
     name          = "openchat/openchat_3.5",
     base_provider = "huggingface",
-    best_provider = RetryProvider([DeepInfra, HuggingChat])
+    best_provider = DeepInfra
 )
 
 # Bard
 gemini = bard = palm = Model(
     name          = 'gemini',
     base_provider = 'google',
     best_provider = Gemini
```

### Comparing `g4f-0.3.0.4/g4f/providers/base_provider.py` & `g4f-0.3.0.5/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/providers/create_images.py` & `g4f-0.3.0.5/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/providers/helper.py` & `g4f-0.3.0.5/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/providers/retry_provider.py` & `g4f-0.3.0.5/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/providers/types.py` & `g4f-0.3.0.5/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/requests/__init__.py` & `g4f-0.3.0.5/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/requests/aiohttp.py` & `g4f-0.3.0.5/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/requests/curl_cffi.py` & `g4f-0.3.0.5/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/requests/defaults.py` & `g4f-0.3.0.5/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/requests/raise_for_status.py` & `g4f-0.3.0.5/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/stubs.py` & `g4f-0.3.0.5/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/typing.py` & `g4f-0.3.0.5/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/version.py` & `g4f-0.3.0.5/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f/webdriver.py` & `g4f-0.3.0.5/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.5/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.4
+Version: 0.3.0.5
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -478,19 +478,20 @@
 | openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://huggingface.co/) |
 | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https://inflection.ai/) |
 
 ### Image and Vision Models
 
 | Label | Provider | Image Model | Vision Model | Website |
 | ----- | -------- | ----------- | ------------ | ------- |
-| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-4-vision | [bing.com](https://bing.com/chat) |
+| Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | gemini| gemini | [gemini.google.com](https://gemini.google.com) |
+| Gemini API | `g4f.Provider.GeminiPro` | ❌| gemini-1.5-pro-latest | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | meta| ❌ | [meta.ai](https://www.meta.ai) |
-| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| ❌ | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) |
 
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.4 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.5 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -368,25 +368,26 @@
 lzlv_70b_fp16_hf | Huggingface | g4f.Provider.DeepInfra | [huggingface.co]
 (https://huggingface.co/) | | airoboros-70b | Huggingface |
 g4f.Provider.DeepInfra | [huggingface.co](https://huggingface.co/) | |
 openchat_3.5 | Huggingface | 2+ Providers | [huggingface.co](https://
 huggingface.co/) | | pi | Inflection | g4f.Provider.Pi | [inflection.ai](https:
 //inflection.ai/) | ### Image and Vision Models | Label | Provider | Image
 Model | Vision Model | Website | | ----- | -------- | ----------- | -----------
-- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e| gpt-
-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
+- | ------- | | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 |
+gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl| llava-1.5-7b-hf | [deepinfra.com]
 (https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` | gemini| gemini |
-[gemini.google.com](https://gemini.google.com) | | Meta AI |
-`g4f.Provider.MetaAI` | meta| â | [meta.ai](https://www.meta.ai) | | OpenAI
-ChatGPT | `g4f.Provider.OpenaiChat` | dall-e| gpt-4-vision | [chat.openai.com]
-(https://chat.openai.com) | | Replicate | `g4f.Provider.Replicate` | stability-
-ai/sdxl| â | [replicate.com](https://replicate.com) | | You.com |
-`g4f.Provider.You` | dall-e| agent | [you.com](https://you.com) | ## ð
-Powered by gpt4free
+[gemini.google.com](https://gemini.google.com) | | Gemini API |
+`g4f.Provider.GeminiPro` | â| gemini-1.5-pro-latest | [ai.google.dev](https:/
+/ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | meta| â | [meta.ai]
+(https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
+`g4f.Provider.Replicate` | stability-ai/sdxl| â | [replicate.com](https://
+replicate.com) | | You.com | `g4f.Provider.You` | dall-e| agent | [you.com]
+(https://you.com) | ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
```

### Comparing `g4f-0.3.0.4/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.5/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/g4f.egg-info/requires.txt` & `g4f-0.3.0.5/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.4/setup.py` & `g4f-0.3.0.5/setup.py`

 * *Files identical despite different names*

