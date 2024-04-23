# Comparing `tmp/nonebot_plugin_manga_translator-0.1.3.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.1.3.tar` & `nonebot_plugin_manga_translator-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/LICENSE
--rw-r--r--   0        0        0     8272 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/README.md
--rw-r--r--   0        0        0     4167 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0     8819 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      529 2023-06-09 12:42:44.263374 nonebot_plugin_manga_translator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9070 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9353 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/README.md
+-rw-r--r--   0        0        0     6922 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0      334 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/config.py
+-rw-r--r--   0        0        0    10693 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      524 2024-04-23 12:17:03.661945 nonebot_plugin_manga_translator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10157 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_manga_translator-0.1.3/LICENSE` & `nonebot_plugin_manga_translator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_manga_translator-0.1.3/README.md` & `nonebot_plugin_manga_translator-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,79 @@
+<!-- markdownlint-disable MD033 -->
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-manga-translator
 
 ✨*基于Nonebot2的图片/漫画翻译插件*✨
 
 <a href="https://github.com/nonebot/nonebot2">
   <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
-</a> 
+</a>
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-manga-translator" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-manga-translator">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-manga-translator" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
-
 <div align="left">
 
 ## 💿安装
+
 通过`pip`或`nb`安装；
 
 - 使用nb:
   在机器人目录下命令行使用
   `nb plugin install nonebot_plugin_manga_translator`
 - 使用pip(不推荐):
-  ~~不推荐就是不推荐，略略略~~
+  `pip install nonebot_plugin_manga_translator`
+  之后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_manga_translator"`
 
 ## 📖简介
 
 1. 适配多种api,将收到的图片翻译并发送翻译后的图片，支持批量操作
 
-2. ⚙️插件配置
+2. 本插件0.2.0版本开始基于[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna/tree/master)插件，适配了多平台（不一定稳定，欢迎提issue或pr），之前的版本只支持onebot.v11适配器
+
+## ⚙️插件配置
+
+### 配置驱动器​
+
+为了适配多平台，从0.2.0以及之后的版本插件需要“客户端型驱动器”（如 httpx）来下载图片等，驱动器安装和配置参考 [NoneBot 选择驱动器](https://nonebot.dev/docs/advanced/driver)
+
+同时需要在 `.env.*` 配置文件中启用对应的驱动器，例如：
+
+```
+DRIVER=~fastapi+~httpx
+```
+
+### 获取API
 
 请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
 ~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
-|          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
-| :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
-|        有道翻译API        |   -   |   -    |                  -                  | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张                   |
-|      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
-|     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
-|        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
-|       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
-|       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
-|        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
-|   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
-| huoshan_secret_access_key |  str  |   ""   |  huoshan_secret_access_key="UT**"   | Secret Access Key |                                                   |
-|        离线翻译API        |   -   |   -    |                  -                  | -                 |                                            可能是电费?       |
-|        offline_url        |  str  |   ""   | offline_url="http://127.0.0.1:5003" | 见下方说明        |                                                   |
-|    其他翻译API(待更新)    |   -   |   -    |                  -                  | -                 |                                                   |
+|          配置项           | 类型  | 默认值 |                 示例                  | 说明              | API定价                                                |
+| :-----------------------: | :---: | :----: | :-----------------------------------: | :---------------- | :----------------------------------------------------- |
+|        有道翻译API        |   -   |   -    |                   -                   | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张 |
+|      youdao_app_key       |  str  |   ""   |        youdao_app_key="xxxxx"         | 应用ID            |                                                        |
+|     youdao_app_secret     |  str  |   ""   |      youdao_app_secret="xxxxxx"       | 应用秘钥          |                                                        |
+|        百度翻译API        |   -   |   -    |                   -                   | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次      |
+|       baidu_app_id        |  str  |   ""   |         baidu_app_id="66666"          | APP ID            |                                                        |
+|       baidu_app_key       |  str  |   ""   |        baidu_app_key="xxxxxx"         | 密钥              |                                                        |
+|        火山翻译API        |   -   |   -    |                   -                   | -                 | 每月前100张免费，之后0.04元/张                         |
+|   huoshan_access_key_id   |  str  |   ""   |     huoshan_access_key_id="AK***"     | Access Key ID     |                                                        |
+| huoshan_secret_access_key |  str  |   ""   |   huoshan_secret_access_key="UT**"    | Secret Access Key |                                                        |
+|        离线翻译API        |   -   |   -    |                   -                   | -                 | 可能是电费?                                            |
+|        offline_url        |  str  |   ""   | offline_url="<http://127.0.0.1:5003>" | 见下方说明        |                                                        |
+|    其他翻译API(待更新)    |   -   |   -    |                   -                   | -                 |                                                        |
 
 ## 🔑API获取
 
 <details>
 <summary>有道翻译</summary>
 
 1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
@@ -109,34 +125,38 @@
 
 1. 图片翻译 [图片]：单张图片翻译，也可以先发送/图片翻译再发送图片,可以如下组合
 
     1. 文字+图片
     2. 先文字，后图片
     3. 文字回复图片
 
-2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息的形式发出,可以如下组合
+2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息（如果平台支持，否则则一张一张发出）的形式发出,可以如下组合
 
-    1. 先文字，后多张图片 
+    1. 先文字，后多张图片
     2. 文字+图片*n
 3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu huoshan offline`
 
 未完待续
 
 ## ⭐效果图
 
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
+![效果图1](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg)
+![效果图2](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg)
+![效果图3](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg)
+![效果图4](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG)
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 2024-04-23:
+
+  - 更新版本，这个版本起开始基于[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna/tree/master)插件支持多适配器多平台(可能有bug)，同时更新nonebot2依赖至2.2.0以上
+
 - 2023-06-09:
 
   - 更新插件元数据
 
 - 2023-05-03:
 
   - 更新说明文档
@@ -155,10 +175,14 @@
 
 ## 🐦计划
 
 - [x] 适配离线翻译模型[manga-image-translator](https://github.com/zyddnys/manga-image-translator)
 
 - [x] 支持更多API
 
+- [x] 多平台适配
+
+- [ ] 支持指定源语言和目标语言
+
 - [ ] 完善插件
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -1,36 +1,47 @@
                                    _[_n_o_n_e_b_o_t_]
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
             æ¼«ç»ç¿»è¯æä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
-nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
-~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
+nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è): `pip install
+nonebot_plugin_manga_translator`
+ä¹åå¨æºå¨äºº`pyproject.toml`éç`plugins =
+[]`åè¡¨è¿½å `"nonebot_plugin_manga_translator"` ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
-2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
+2. æ¬æä»¶0.2.0çæ¬å¼å§åºäº[nonebot-plugin-alconna](https://github.com/
+nonebot/plugin-alconna/tree/
+master)æä»¶ï¼ééäºå¤å¹³å°ï¼ä¸ä¸å®ç¨³å®ï¼æ¬¢è¿æissueæprï¼ï¼ä¹åççæ¬åªæ¯æonebot.v11ééå¨
+## âï¸æä»¶éç½® ### éç½®é©±å¨å¨â
+ä¸ºäºééå¤å¹³å°ï¼ä»0.2.0ä»¥åä¹åççæ¬æä»¶éè¦âå®¢æ·ç«¯åé©±å¨å¨âï¼å¦
+httpxï¼æ¥ä¸è½½å¾çç­ï¼é©±å¨å¨å®è£åéç½®åè [NoneBot
+éæ©é©±å¨å¨](https://nonebot.dev/docs/advanced/driver) åæ¶éè¦å¨
+`.env.*` éç½®æä»¶ä¸­å¯ç¨å¯¹åºçé©±å¨å¨ï¼ä¾å¦ï¼ ```
+DRIVER=~fastapi+~httpx ``` ### è·åAPI
+è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
 (è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
 ~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
-------------: | :---: | :----: | :---------------------------------: | :-------
---------- | :------------------------------------------------ | |
+------------: | :---: | :----: | :-----------------------------------: | :-----
+----------- | :----------------------------------------------------- | |
 æéç¿»è¯API | - | - | - | - | æ°ç¨æ·éä¸å®é¢åº¦,æ¢¯åº¦æ¶è´¹ï¼0
 è°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | "" |
 youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
 youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
 | æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
 baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
 str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
 - | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
 "" | huoshan_access_key_id="AK***" | Access Key ID | | |
 huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
 Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
-offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
-| | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | | ## ðAPIè·å
-æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
-)æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
+offline_url | str | "" | offline_url="
+127.0.0.1:5003>" | è§ä¸æ¹è¯´æ | | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | -
+| - | | ## ðAPIè·å æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https:
+//ai.youdao.com/#/)æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
 å¨å·¦ä¾§`èªç¶è¯­è¨ç¿»è¯æå¡`éç`å¾çç¿»è¯`éåå»ºåºç¨ï¼éæ©æå¡åæ¥å¥æ¹å¼åå«ä¸º`å¾çç¿»è¯`å`API`ï¼å¶ä»é¡¹éæã
 ![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
 main/resource/æéç¿»è¯.png) 3.
 åå»ºåå°`åºç¨ID`å`åºç¨ç§é¥`æç§ä¸é¢çéç½®è¯´æåå«å¡«å¥.env.*æä»¶éå³å¯
 ç¾åº¦ç¿»è¯ 1. å¨[ç¾åº¦ç¿»è¯å¼æ¾å¹³å°](https://api.fanyi.baidu.com/
 )æ³¨åå¹¶ç»å½ 2. æ¾å°`äº§åæå¡`ç`å¾çç¿»è¯`,ç³è¯·åå»º 3.
 åå»ºåå¨`ç®¡çæ§å¶å°`ç`æ»è§`ä¸­æ¾å°`APP
@@ -59,26 +70,31 @@
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
 README.md),ä¿®æ¹å­å¸`data`ï¼ä»èæå®ä½ æ³è¦çOCRæ¨¡ååç¿»è¯æ¨¡å
 (ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç) ## ðå½ä»¤ 1.
 å¾çç¿»è¯ [å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
 å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
 åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
-[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
+[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯ï¼å¦æå¹³å°æ¯æï¼å¦ååä¸å¼ ä¸å¼ ååºï¼çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
 1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
 å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
-æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
-translator/blob/main/resource/ææå¾1.jpg][https://github.com/maoxig/
-nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg][https://
-github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
-ææå¾3.jpg][https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
-main/resource/ææå¾4.PNG]## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2023-06-09: -
+æªå®å¾ç»­ ## â­ææå¾ ![ææå¾1](https://github.com/maoxig/nonebot-
+plugin-manga-translator/blob/main/resource/ææå¾1.jpg) ![ææå¾2](https:
+//github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
+ææå¾2.jpg) ![ææå¾3](https://github.com/maoxig/nonebot-plugin-manga-
+translator/blob/main/resource/ææå¾3.jpg) ![ææå¾4](https://github.com/
+maoxig/nonebot-plugin-manga-translator/blob/main/resource/ææå¾4.PNG) ##
+ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2024-04-23: -
+æ´æ°çæ¬ï¼è¿ä¸ªçæ¬èµ·å¼å§åºäº[nonebot-plugin-alconna](https://
+github.com/nonebot/plugin-alconna/tree/master)æä»¶æ¯æå¤ééå¨å¤å¹³å°
+(å¯è½æbug)ï¼åæ¶æ´æ°nonebot2ä¾èµè³2.2.0ä»¥ä¸ - 2023-06-09: -
 æ´æ°æä»¶åæ°æ® - 2023-05-03: - æ´æ°è¯´æææ¡£ - éé
 [ç«å±±ç¿»è¯api](https://translate.volcengine.com/
 api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI - 2023-05-01: -
 æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
 ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
 image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
 æä»¶åå¸ ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
 translator](https://github.com/zyddnys/manga-image-translator) - [x]
-æ¯ææ´å¤API - [ ] å®åæä»¶ ##
+æ¯ææ´å¤API - [x] å¤å¹³å°éé - [ ]
+æ¯ææå®æºè¯­è¨åç®æ è¯­è¨ - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

### Comparing `nonebot_plugin_manga_translator-0.1.3/nonebot_plugin_manga_translator/utils.py` & `nonebot_plugin_manga_translator-0.2.0/nonebot_plugin_manga_translator/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,199 +3,281 @@
 import base64
 import random
 from hashlib import md5
 from PIL import Image
 from io import BytesIO
 from nonebot import logger
 import asyncio
-from pydantic import BaseModel,Extra
 import time
 import json
 import datetime
 import hashlib
 import hmac
 from urllib.parse import quote
-class Config(BaseModel,extra=Extra.ignore):
-    #百度
-    baidu_app_id:str=""
-    baidu_app_key:str=""
-    #有道
-    youdao_app_key:str=""
-    youdao_app_secret:str=""
-    #离线
-    offline_url:str=""
-    #火山翻译
-    huoshan_access_key_id:str=""
-    huoshan_secret_access_key:str=""
 
 
 class MangaTranslator:
-    
-    def __init__(self,driver:dict) -> None:
-        self.config=Config.parse_obj(driver)
-        self.img_url=[]
-        self.api=[]
+
+    def __init__(self, Config) -> None:
+        self.config = Config
+        self.img_url = []
+        self.api = []
         if self.config.youdao_app_key:
             self.api.append(self.youdao)
             logger.info("检测到有道API")
         if self.config.baidu_app_id:
             self.api.append(self.baidu)
             logger.info("检测到百度API")
         if self.config.offline_url:
             self.api.append(self.offline)
             logger.info("检测到离线模型")
         if self.config.huoshan_access_key_id:
             self.api.append(self.huoshan)
             logger.info("检测到火山API")
-            
-    async def call_api(self,imageUrl):
+
+    async def call_api(self, image_bytes):
         for api in self.api:
             try:
-                result=await api(imageUrl)
+                result = await api(image_bytes)
                 return result
             except httpx.HTTPError as e:
                 logger.warning(f"API[{api.__name__}]不可用：{e}尝试切换下一个")
-        return None,"无可用API"
-   
- 
-    async def youdao(self,imageUrl):
+        return None, "无可用API"
+
+    async def youdao(self, image_bytes):
         """有道翻译"""
         salt = str(uuid.uuid1())
-        data = {'from': 'auto', 'to': 'zh-CHS', 'type': '1','appKey': self.config.youdao_app_key, 'salt': salt, "render": 1}
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        data = {
+            "from": "auto",
+            "to": "zh-CHS",
+            "type": "1",
+            "appKey": self.config.youdao_app_key,
+            "salt": salt,
+            "render": 1,
+        }
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
         async with httpx.AsyncClient() as client:
-            res=await client.get(imageUrl)
-            if len(res.content)>=2*1024*1024:
-                res.content=self.compress_image(res.content)
-            q=base64.b64encode(res.content).decode("utf-8")
-            data['q'] = q
-            signStr = self.config.youdao_app_key + q + salt + self.config.youdao_app_secret
+            if len(image_bytes) >= 2 * 1024 * 1024:
+                image_bytes = self.compress_image(image_bytes)
+            q = base64.b64encode(image_bytes).decode("utf-8")
+            data["q"] = q
+            signStr = (
+                self.config.youdao_app_key + q + salt + self.config.youdao_app_secret
+            )
             sign = self.encrypt(signStr)
-            data['sign'] = sign
-            youdao_res=await client.post(url='https://openapi.youdao.com/ocrtransapi',data=data,headers=headers)
-            img_base64=youdao_res.json()["render_image"]
-            pic=base64.b64decode(img_base64)
-        return pic,"有道"
-    
-    
-    async def baidu(self,imageUrl):
+            data["sign"] = sign
+            youdao_res = await client.post(
+                url="https://openapi.youdao.com/ocrtransapi", data=data, headers=headers
+            )
+            img_base64 = youdao_res.json()["render_image"]
+            pic = base64.b64decode(img_base64)
+        return pic, "有道"
+
+    async def baidu(self, image_bytes):
         """百度翻译"""
         async with httpx.AsyncClient() as client:
-            res=await client.get(imageUrl)
             salt = random.randint(32768, 65536)
-            image_data=res.content
-            image_size=len(image_data)
-            if image_size>=4*1024*1024:
+            image_data = image_bytes
+            image_size = len(image_data)
+            if image_size >= 4 * 1024 * 1024:
                 logger.info("图片过大，进行压缩")
-                image_data=self.compress_image(image_data)
-            sign = md5((self.config.baidu_app_id+md5(image_data).hexdigest()+str(salt)+"APICUID"+"mac"+self.config.baidu_app_key).encode('utf-8')).hexdigest()
-            payload = {'from': "auto", 'to': "zh", 'appid': self.config.baidu_app_id, 'salt': salt, 'sign': sign, 'cuid': 'APICUID', 'mac': "mac","paste":1,"version":3}
-            image = {'image': ("image.jpg",image_data, "multipart/form-data")}
-            baidu_res=await client.post(url='http://api.fanyi.baidu.com/api/trans/sdk/picture',params=payload,files=image)
-            img_base64=baidu_res.json()["data"]["pasteImg"]
-            pic=base64.b64decode(img_base64)
-        return pic,"百度"
-    
+                image_data = self.compress_image(image_data)
+            sign = md5(
+                (
+                    self.config.baidu_app_id
+                    + md5(image_data).hexdigest()
+                    + str(salt)
+                    + "APICUID"
+                    + "mac"
+                    + self.config.baidu_app_key
+                ).encode("utf-8")
+            ).hexdigest()
+            payload = {
+                "from": "auto",
+                "to": "zh",
+                "appid": self.config.baidu_app_id,
+                "salt": salt,
+                "sign": sign,
+                "cuid": "APICUID",
+                "mac": "mac",
+                "paste": 1,
+                "version": 3,
+            }
+            image = {"image": ("image.jpg", image_data, "multipart/form-data")}
+            baidu_res = await client.post(
+                url="http://api.fanyi.baidu.com/api/trans/sdk/picture",
+                params=payload,
+                files=image,
+            )
+            img_base64 = baidu_res.json()["data"]["pasteImg"]
+            pic = base64.b64decode(img_base64)
+        return pic, "百度"
 
-    async def offline(self, imgUrl, timeout=60):
+    async def offline(self, image_bytes, timeout=60):
         """离线翻译,这里写的有点烂，求pr"""
         async with httpx.AsyncClient() as client:
-            res = await client.get(imgUrl)
-            img_content = res.content
-            form = {"file": ("image.png", img_content, 'image/png')}
-            response = await client.post(self.config.offline_url + "/submit", files=form,data={"translator":"offline"})#改为本地翻译器
-            #这里的填写请参考文档，根据自己情况填写，例如data={"translator":"youdao","tgt_lang":"CHS"},如果是有道、百度、gpt等，请确保填写了key
+            img_content = image_bytes
+            form = {"file": ("image.png", img_content, "image/png")}
+            response = await client.post(
+                self.config.offline_url + "/submit",
+                files=form,
+                data={"translator": "offline"},
+            )  # 改为本地翻译器
+            # 这里的填写请参考文档，根据自己情况填写，例如data={"translator":"youdao","tgt_lang":"CHS"},如果是有道、百度、gpt等，请确保填写了key
             response.raise_for_status()  # 检查响应状态
             task_id = response.json()["task_id"]
             req = {"taskid": task_id}
             # 轮询获取翻译结果，超时时间为60s
             start_time = time.monotonic()
             while True:
-                response = await client.get(self.config.offline_url + "/task-state", params=req)
+                response = await client.get(
+                    self.config.offline_url + "/task-state", params=req
+                )
                 logger.debug(response.content)
                 response.raise_for_status()
                 state = response.json()["state"]
-                finished=response.json()["finished"]
+                finished = response.json()["finished"]
                 if state == "finished" or finished:
                     break
                 if time.monotonic() - start_time > timeout:
                     return None, "超时"
                 await asyncio.sleep(1)
-            img_data = await client.get(url=self.config.offline_url+"/result/"+task_id)
+            img_data = await client.get(
+                url=self.config.offline_url + "/result/" + task_id
+            )
             if img_data.status_code == 200 and img_data.content:
                 return img_data.content, "离线"
             else:
                 return None, "离线"
 
-
-    async def huoshan(self,imageUrl):
+    async def huoshan(self, image_bytes):
         """火山引擎翻译，构建签名"""
         async with httpx.AsyncClient() as client:
-            res=await client.get(imageUrl)
-            data=json.dumps({"Image":str(base64.b64encode(res.content),encoding='utf-8'),'TargetLanguage': "zh"})
-            x_content_sha256=self.hash_sha256(data)
-            now_time=datetime.datetime.utcnow()#
-            x_date=now_time.strftime("%Y%m%dT%H%M%SZ")
-            credential_scope = "/".join([x_date[:8], "cn-north-1", 'translate', "request"])
+            data = json.dumps(
+                {
+                    "Image": str(base64.b64encode(image_bytes), encoding="utf-8"),
+                    "TargetLanguage": "zh",
+                }
+            )
+            x_content_sha256 = self.hash_sha256(data)
+            now_time = datetime.datetime.utcnow()  #
+            x_date = now_time.strftime("%Y%m%dT%H%M%SZ")
+            credential_scope = "/".join(
+                [x_date[:8], "cn-north-1", "translate", "request"]
+            )
             signed_headers_str = ";".join(
-            ["content-type", "host", "x-content-sha256", "x-date"])
+                ["content-type", "host", "x-content-sha256", "x-date"]
+            )
             canonical_request_str = "\n".join(
-            ["POST",
-            "/",
-            self.norm_query({'Action': 'TranslateImage','Version': '2020-07-01'}),
-            "\n".join(["content-type:" + 'application/json',"host:" + 'open.volcengineapi.com',"x-content-sha256:" + x_content_sha256,"x-date:" + x_date,]),
-            "",
-            signed_headers_str,
-            x_content_sha256,
-            ])
-            sign_result={
-            "Host":"open.volcengineapi.com",
-            "X-Content-Sha256": x_content_sha256,
-            "X-Date": x_date,
-            "Content-Type": 'application/json',
-            "Authorization": "HMAC-SHA256 Credential={}, SignedHeaders={}, Signature={}".format(
-            self.config.huoshan_access_key_id + "/" + credential_scope,
-            signed_headers_str,
-            self.hmac_sha256(self.hmac_sha256(self.hmac_sha256(self.hmac_sha256(self.hmac_sha256(self.config.huoshan_secret_access_key.encode("utf-8"), x_date[:8]), 'cn-north-1'),'translate'), "request"),"\n".join(["HMAC-SHA256", x_date, credential_scope,self.hash_sha256(canonical_request_str)])).hex()
+                [
+                    "POST",
+                    "/",
+                    self.norm_query(
+                        {"Action": "TranslateImage", "Version": "2020-07-01"}
+                    ),
+                    "\n".join(
+                        [
+                            "content-type:" + "application/json",
+                            "host:" + "open.volcengineapi.com",
+                            "x-content-sha256:" + x_content_sha256,
+                            "x-date:" + x_date,
+                        ]
+                    ),
+                    "",
+                    signed_headers_str,
+                    x_content_sha256,
+                ]
             )
+            sign_result = {
+                "Host": "open.volcengineapi.com",
+                "X-Content-Sha256": x_content_sha256,
+                "X-Date": x_date,
+                "Content-Type": "application/json",
+                "Authorization": "HMAC-SHA256 Credential={}, SignedHeaders={}, Signature={}".format(
+                    self.config.huoshan_access_key_id + "/" + credential_scope,
+                    signed_headers_str,
+                    self.hmac_sha256(
+                        self.hmac_sha256(
+                            self.hmac_sha256(
+                                self.hmac_sha256(
+                                    self.hmac_sha256(
+                                        self.config.huoshan_secret_access_key.encode(
+                                            "utf-8"
+                                        ),
+                                        x_date[:8],
+                                    ),
+                                    "cn-north-1",
+                                ),
+                                "translate",
+                            ),
+                            "request",
+                        ),
+                        "\n".join(
+                            [
+                                "HMAC-SHA256",
+                                x_date,
+                                credential_scope,
+                                self.hash_sha256(canonical_request_str),
+                            ]
+                        ),
+                    ).hex(),
+                ),
             }
-            params={"Action": 'TranslateImage', "Version":'2020-07-01' }
-            huoshan_res=await client.post(url='https://open.volcengineapi.com/',headers=sign_result,params=params,data=data)
-            img_base64=huoshan_res.json()["Image"]
-            pic=base64.b64decode(img_base64)
-        return pic,"火山"
+            params = {"Action": "TranslateImage", "Version": "2020-07-01"}
+            huoshan_res = await client.post(
+                url="https://open.volcengineapi.com/",
+                headers=sign_result,
+                params=params,
+                data=data,
+            )
+            img_base64 = huoshan_res.json()["Image"]
+            pic = base64.b64decode(img_base64)
+        return pic, "火山"
 
-            
     @staticmethod
     def compress_image(image_data):
         with BytesIO(image_data) as input:
-            image=Image.open(input)
-            image=image.convert("RGB")
-            image=image.resize((int(image.width*0.5),int(image.height*0.5)),Image.ANTIALIAS)
-            image.save(input,format="JPEG",quality=80)
+            image = Image.open(input)
+            image = image.convert("RGB")
+            image = image.resize(
+                (int(image.width * 0.5), int(image.height * 0.5)), Image.ANTIALIAS
+            )
+            image.save(input, format="JPEG", quality=80)
             return input.getvalue()
-        
+
     @staticmethod
     def encrypt(signStr):
         hash_algorithm = md5()
-        hash_algorithm.update(signStr.encode('utf-8'))
+        hash_algorithm.update(signStr.encode("utf-8"))
         return hash_algorithm.hexdigest()
-    
+
     @staticmethod
     def hash_sha256(content: str):
         return hashlib.sha256(content.encode("utf-8")).hexdigest()
-    
+
     @staticmethod
     def norm_query(params):
         query = ""
         for key in sorted(params.keys()):
-            if type(params[key]) == list:
+            if isinstance(params[key], list):
                 for k in params[key]:
-                    query = (query + quote(key, safe="-_.~") + "=" + quote(k, safe="-_.~") + "&")
+                    query = (
+                        query
+                        + quote(key, safe="-_.~")
+                        + "="
+                        + quote(k, safe="-_.~")
+                        + "&"
+                    )
             else:
-                query = (query + quote(key, safe="-_.~") + "=" + quote(params[key], safe="-_.~") + "&")
+                query = (
+                    query
+                    + quote(key, safe="-_.~")
+                    + "="
+                    + quote(params[key], safe="-_.~")
+                    + "&"
+                )
         query = query[:-1]
         return query.replace("+", "%20")
-    
+
     @staticmethod
     def hmac_sha256(key: bytes, content: str):
         return hmac.new(key, content.encode("utf-8"), hashlib.sha256).digest()
```

### Comparing `nonebot_plugin_manga_translator-0.1.3/PKG-INFO` & `nonebot_plugin_manga_translator-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,100 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-manga-translator
-Version: 0.1.3
+Version: 0.2.0
 Summary: 基于nonebot2的适配多种api的图片/漫画翻译插件
 License: MIT
 Author: xenophon
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot-plugin-alconna (>=0.40.1,<1.0.0)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
+<!-- markdownlint-disable MD033 -->
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-manga-translator
 
 ✨*基于Nonebot2的图片/漫画翻译插件*✨
 
 <a href="https://github.com/nonebot/nonebot2">
   <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
-</a> 
+</a>
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-manga-translator" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-manga-translator">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-manga-translator" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
-
 <div align="left">
 
 ## 💿安装
+
 通过`pip`或`nb`安装；
 
 - 使用nb:
   在机器人目录下命令行使用
   `nb plugin install nonebot_plugin_manga_translator`
 - 使用pip(不推荐):
-  ~~不推荐就是不推荐，略略略~~
+  `pip install nonebot_plugin_manga_translator`
+  之后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_manga_translator"`
 
 ## 📖简介
 
 1. 适配多种api,将收到的图片翻译并发送翻译后的图片，支持批量操作
 
-2. ⚙️插件配置
+2. 本插件0.2.0版本开始基于[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna/tree/master)插件，适配了多平台（不一定稳定，欢迎提issue或pr），之前的版本只支持onebot.v11适配器
+
+## ⚙️插件配置
+
+### 配置驱动器​
+
+为了适配多平台，从0.2.0以及之后的版本插件需要“客户端型驱动器”（如 httpx）来下载图片等，驱动器安装和配置参考 [NoneBot 选择驱动器](https://nonebot.dev/docs/advanced/driver)
+
+同时需要在 `.env.*` 配置文件中启用对应的驱动器，例如：
+
+```
+DRIVER=~fastapi+~httpx
+```
+
+### 获取API
 
 请在机器人目录下的.env.*里填写以下选项(至少填一个平台的)，获取方式已整理好，见下方
 
 ~~个人感觉就漫画翻译而言,这几家API的效果大致为有道>=百度≈离线>=火山,且火山翻译对竖版日文的翻译效果很差~~
 
-|          配置项           | 类型  | 默认值 |                示例                 | 说明              | API定价                                           |
-| :-----------------------: | :---: | :----: | :---------------------------------: | :---------------- | :------------------------------------------------ |
-|        有道翻译API        |   -   |   -    |                  -                  | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张                   |
-|      youdao_app_key       |  str  |   ""   |       youdao_app_key="xxxxx"        | 应用ID            |                                                   |
-|     youdao_app_secret     |  str  |   ""   |     youdao_app_secret="xxxxxx"      | 应用秘钥          |                                                   |
-|        百度翻译API        |   -   |   -    |                  -                  | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次 |
-|       baidu_app_id        |  str  |   ""   |        baidu_app_id="66666"         | APP ID            |                                                   |
-|       baidu_app_key       |  str  |   ""   |       baidu_app_key="xxxxxx"        | 密钥              |                                                   |
-|        火山翻译API        |   -   |   -    |                  -                  | -                 | 每月前100张免费，之后0.04元/张                    |
-|   huoshan_access_key_id   |  str  |   ""   |    huoshan_access_key_id="AK***"    | Access Key ID     |                                                   |
-| huoshan_secret_access_key |  str  |   ""   |  huoshan_secret_access_key="UT**"   | Secret Access Key |                                                   |
-|        离线翻译API        |   -   |   -    |                  -                  | -                 |                                            可能是电费?       |
-|        offline_url        |  str  |   ""   | offline_url="http://127.0.0.1:5003" | 见下方说明        |                                                   |
-|    其他翻译API(待更新)    |   -   |   -    |                  -                  | -                 |                                                   |
+|          配置项           | 类型  | 默认值 |                 示例                  | 说明              | API定价                                                |
+| :-----------------------: | :---: | :----: | :-----------------------------------: | :---------------- | :----------------------------------------------------- |
+|        有道翻译API        |   -   |   -    |                   -                   | -                 | 新用户送一定额度,梯度收费，0<月调用量<100w时,0.04元/张 |
+|      youdao_app_key       |  str  |   ""   |        youdao_app_key="xxxxx"         | 应用ID            |                                                        |
+|     youdao_app_secret     |  str  |   ""   |      youdao_app_secret="xxxxxx"       | 应用秘钥          |                                                        |
+|        百度翻译API        |   -   |   -    |                   -                   | -                 | 每月1万次免费调用量，之后按梯度收费,最高0.04元/次      |
+|       baidu_app_id        |  str  |   ""   |         baidu_app_id="66666"          | APP ID            |                                                        |
+|       baidu_app_key       |  str  |   ""   |        baidu_app_key="xxxxxx"         | 密钥              |                                                        |
+|        火山翻译API        |   -   |   -    |                   -                   | -                 | 每月前100张免费，之后0.04元/张                         |
+|   huoshan_access_key_id   |  str  |   ""   |     huoshan_access_key_id="AK***"     | Access Key ID     |                                                        |
+| huoshan_secret_access_key |  str  |   ""   |   huoshan_secret_access_key="UT**"    | Secret Access Key |                                                        |
+|        离线翻译API        |   -   |   -    |                   -                   | -                 | 可能是电费?                                            |
+|        offline_url        |  str  |   ""   | offline_url="<http://127.0.0.1:5003>" | 见下方说明        |                                                        |
+|    其他翻译API(待更新)    |   -   |   -    |                   -                   | -                 |                                                        |
 
 ## 🔑API获取
 
 <details>
 <summary>有道翻译</summary>
 
 1. 在[有道智云AI开放平台](https://ai.youdao.com/#/)注册并登录后，进入控制台
@@ -130,34 +146,38 @@
 
 1. 图片翻译 [图片]：单张图片翻译，也可以先发送/图片翻译再发送图片,可以如下组合
 
     1. 文字+图片
     2. 先文字，后图片
     3. 文字回复图片
 
-2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息的形式发出,可以如下组合
+2. 多图片翻译 [图片]：n张图片翻译，将会以合并转发消息（如果平台支持，否则则一张一张发出）的形式发出,可以如下组合
 
-    1. 先文字，后多张图片 
+    1. 先文字，后多张图片
     2. 文字+图片*n
 3. 切换翻译api [api]: 将该api优先级提到最高，目前有`youdao baidu huoshan offline`
 
 未完待续
 
 ## ⭐效果图
 
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg" width="300" height="300">
-<img src="https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG" width="300" height="300">
+![效果图1](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图1.jpg)
+![效果图2](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图2.jpg)
+![效果图3](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图3.jpg)
+![效果图4](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/效果图4.PNG)
 
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 2024-04-23:
+
+  - 更新版本，这个版本起开始基于[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna/tree/master)插件支持多适配器多平台(可能有bug)，同时更新nonebot2依赖至2.2.0以上
+
 - 2023-06-09:
 
   - 更新插件元数据
 
 - 2023-05-03:
 
   - 更新说明文档
@@ -176,11 +196,15 @@
 
 ## 🐦计划
 
 - [x] 适配离线翻译模型[manga-image-translator](https://github.com/zyddnys/manga-image-translator)
 
 - [x] 支持更多API
 
+- [x] 多平台适配
+
+- [ ] 支持指定源语言和目标语言
+
 - [ ] 完善插件
 
 ## ✨喜欢的话就点个star✨吧，球球了QAQ
```

#### html2text {}

```diff
@@ -1,47 +1,58 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-manga-translator Version: 0.2.0
 Summary: åºäºnonebot2çééå¤ç§apiçå¾ç/æ¼«ç»ç¿»è¯æä»¶ License:
 MIT Author: xenophon Author-email: 674550338@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=9.1.1,<10.0.0) Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot2
-(>=2.0.0rc1,<3.0.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Description-
-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Pillow
+(>=9.1.1,<10.0.0) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist:
+nonebot-plugin-alconna (>=0.40.1,<1.0.0) Requires-Dist: nonebot2
+(>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
         # nonebot-plugin-manga-translator â¨*åºäºNonebot2çå¾ç/
             æ¼«ç»ç¿»è¯æä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð¿å®è£ éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb:
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨ `nb plugin install
-nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è):
-~~ä¸æ¨èå°±æ¯ä¸æ¨èï¼ç¥ç¥ç¥~~ ## ðç®ä» 1.
+nonebot_plugin_manga_translator` - ä½¿ç¨pip(ä¸æ¨è): `pip install
+nonebot_plugin_manga_translator`
+ä¹åå¨æºå¨äºº`pyproject.toml`éç`plugins =
+[]`åè¡¨è¿½å `"nonebot_plugin_manga_translator"` ## ðç®ä» 1.
 ééå¤ç§api,å°æ¶å°çå¾çç¿»è¯å¹¶åéç¿»è¯åçå¾çï¼æ¯ææ¹éæä½
-2. âï¸æä»¶éç½® è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
+2. æ¬æä»¶0.2.0çæ¬å¼å§åºäº[nonebot-plugin-alconna](https://github.com/
+nonebot/plugin-alconna/tree/
+master)æä»¶ï¼ééäºå¤å¹³å°ï¼ä¸ä¸å®ç¨³å®ï¼æ¬¢è¿æissueæprï¼ï¼ä¹åççæ¬åªæ¯æonebot.v11ééå¨
+## âï¸æä»¶éç½® ### éç½®é©±å¨å¨â
+ä¸ºäºééå¤å¹³å°ï¼ä»0.2.0ä»¥åä¹åççæ¬æä»¶éè¦âå®¢æ·ç«¯åé©±å¨å¨âï¼å¦
+httpxï¼æ¥ä¸è½½å¾çç­ï¼é©±å¨å¨å®è£åéç½®åè [NoneBot
+éæ©é©±å¨å¨](https://nonebot.dev/docs/advanced/driver) åæ¶éè¦å¨
+`.env.*` éç½®æä»¶ä¸­å¯ç¨å¯¹åºçé©±å¨å¨ï¼ä¾å¦ï¼ ```
+DRIVER=~fastapi+~httpx ``` ### è·åAPI
+è¯·å¨æºå¨äººç®å½ä¸ç.env.*éå¡«åä»¥ä¸éé¡¹
 (è³å°å¡«ä¸ä¸ªå¹³å°ç)ï¼è·åæ¹å¼å·²æ´çå¥½ï¼è§ä¸æ¹
 ~~ä¸ªäººæè§å°±æ¼«ç»ç¿»è¯èè¨,è¿å å®¶APIçææå¤§è´ä¸ºæé>=ç¾åº¦âç¦»çº¿>=ç«å±±,ä¸ç«å±±ç¿»è¯å¯¹ç«çæ¥æçç¿»è¯ææå¾å·®~~
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | ç¤ºä¾ | è¯´æ | APIå®ä»· | | :-----------
-------------: | :---: | :----: | :---------------------------------: | :-------
---------- | :------------------------------------------------ | |
+------------: | :---: | :----: | :-----------------------------------: | :-----
+----------- | :----------------------------------------------------- | |
 æéç¿»è¯API | - | - | - | - | æ°ç¨æ·éä¸å®é¢åº¦,æ¢¯åº¦æ¶è´¹ï¼0
 è°ç¨é<100wæ¶,0.04å/å¼  | | youdao_app_key | str | "" |
 youdao_app_key="xxxxx" | åºç¨ID | | | youdao_app_secret | str | "" |
 youdao_app_secret="xxxxxx" | åºç¨ç§é¥ | | | ç¾åº¦ç¿»è¯API | - | - | - | -
 | æ¯æ1ä¸æ¬¡åè´¹è°ç¨éï¼ä¹åææ¢¯åº¦æ¶è´¹,æé«0.04å/æ¬¡ | |
 baidu_app_id | str | "" | baidu_app_id="66666" | APP ID | | | baidu_app_key |
 str | "" | baidu_app_key="xxxxxx" | å¯é¥ | | | ç«å±±ç¿»è¯API | - | - | - |
 - | æ¯æå100å¼ åè´¹ï¼ä¹å0.04å/å¼  | | huoshan_access_key_id | str |
 "" | huoshan_access_key_id="AK***" | Access Key ID | | |
 huoshan_secret_access_key | str | "" | huoshan_secret_access_key="UT**" |
 Secret Access Key | | | ç¦»çº¿ç¿»è¯API | - | - | - | - | å¯è½æ¯çµè´¹? | |
-offline_url | str | "" | offline_url="http://127.0.0.1:5003" | è§ä¸æ¹è¯´æ
-| | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | - | - | | ## ðAPIè·å
-æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https://ai.youdao.com/#/
-)æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
+offline_url | str | "" | offline_url="
+127.0.0.1:5003>" | è§ä¸æ¹è¯´æ | | | å¶ä»ç¿»è¯API(å¾æ´æ°) | - | - | -
+| - | | ## ðAPIè·å æéç¿»è¯ 1. å¨[æéæºäºAIå¼æ¾å¹³å°](https:
+//ai.youdao.com/#/)æ³¨åå¹¶ç»å½åï¼è¿å¥æ§å¶å° 2.
 å¨å·¦ä¾§`èªç¶è¯­è¨ç¿»è¯æå¡`éç`å¾çç¿»è¯`éåå»ºåºç¨ï¼éæ©æå¡åæ¥å¥æ¹å¼åå«ä¸º`å¾çç¿»è¯`å`API`ï¼å¶ä»é¡¹éæã
 ![Image text](https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
 main/resource/æéç¿»è¯.png) 3.
 åå»ºåå°`åºç¨ID`å`åºç¨ç§é¥`æç§ä¸é¢çéç½®è¯´æåå«å¡«å¥.env.*æä»¶éå³å¯
 ç¾åº¦ç¿»è¯ 1. å¨[ç¾åº¦ç¿»è¯å¼æ¾å¹³å°](https://api.fanyi.baidu.com/
 )æ³¨åå¹¶ç»å½ 2. æ¾å°`äº§åæå¡`ç`å¾çç¿»è¯`,ç³è¯·åå»º 3.
 åå»ºåå¨`ç®¡çæ§å¶å°`ç`æ»è§`ä¸­æ¾å°`APP
@@ -70,26 +81,31 @@
 æåä½ **å¯è½**è¿éè¦ä¿®æ¹ä¸ä¸æ¬æä»¶çä»£ç ï¼æ¾å°æ¬æä»¶`utils.py`ç`offline`å½æ°ï¼æ ¹æ®æ³¨éå
 [ææ¡£](https://github.com/zyddnys/manga-image-translator/blob/main/
 README.md),ä¿®æ¹å­å¸`data`ï¼ä»èæå®ä½ æ³è¦çOCRæ¨¡ååç¿»è¯æ¨¡å
 (ç®åæ¯ç¨äºofflineæ¨¡å,ä½ å¯ä»¥æ¹æå«ç) ## ðå½ä»¤ 1.
 å¾çç¿»è¯ [å¾ç]ï¼åå¼ å¾çç¿»è¯ï¼ä¹å¯ä»¥ååé/
 å¾çç¿»è¯ååéå¾ç,å¯ä»¥å¦ä¸ç»å 1. æå­+å¾ç 2.
 åæå­ï¼åå¾ç 3. æå­åå¤å¾ç 2. å¤å¾çç¿»è¯
-[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
+[å¾ç]ï¼nå¼ å¾çç¿»è¯ï¼å°ä¼ä»¥åå¹¶è½¬åæ¶æ¯ï¼å¦æå¹³å°æ¯æï¼å¦ååä¸å¼ ä¸å¼ ååºï¼çå½¢å¼ååº,å¯ä»¥å¦ä¸ç»å
 1. åæå­ï¼åå¤å¼ å¾ç 2. æå­+å¾ç*n 3. åæ¢ç¿»è¯api [api]:
 å°è¯¥apiä¼åçº§æå°æé«ï¼ç®åæ`youdao baidu huoshan offline`
-æªå®å¾ç»­ ## â­ææå¾ [https://github.com/maoxig/nonebot-plugin-manga-
-translator/blob/main/resource/ææå¾1.jpg][https://github.com/maoxig/
-nonebot-plugin-manga-translator/blob/main/resource/ææå¾2.jpg][https://
-github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
-ææå¾3.jpg][https://github.com/maoxig/nonebot-plugin-manga-translator/blob/
-main/resource/ææå¾4.PNG]## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2023-06-09: -
+æªå®å¾ç»­ ## â­ææå¾ ![ææå¾1](https://github.com/maoxig/nonebot-
+plugin-manga-translator/blob/main/resource/ææå¾1.jpg) ![ææå¾2](https:
+//github.com/maoxig/nonebot-plugin-manga-translator/blob/main/resource/
+ææå¾2.jpg) ![ææå¾3](https://github.com/maoxig/nonebot-plugin-manga-
+translator/blob/main/resource/ææå¾3.jpg) ![ææå¾4](https://github.com/
+maoxig/nonebot-plugin-manga-translator/blob/main/resource/ææå¾4.PNG) ##
+ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2024-04-23: -
+æ´æ°çæ¬ï¼è¿ä¸ªçæ¬èµ·å¼å§åºäº[nonebot-plugin-alconna](https://
+github.com/nonebot/plugin-alconna/tree/master)æä»¶æ¯æå¤ééå¨å¤å¹³å°
+(å¯è½æbug)ï¼åæ¶æ´æ°nonebot2ä¾èµè³2.2.0ä»¥ä¸ - 2023-06-09: -
 æ´æ°æä»¶åæ°æ® - 2023-05-03: - æ´æ°è¯´æææ¡£ - éé
 [ç«å±±ç¿»è¯api](https://translate.volcengine.com/
 api),ä½ å¯ä»¥éæ©æ¥å¥ç«å±±ç¿»è¯æä¾çAPI - 2023-05-01: -
 æ·»å åæ¢apiçåè½ï¼ä½ å¯ä»¥å°æä¸ªapiä¼åçº§è®¾ä¸ºæé« -
 ééç¦»çº¿ç¿»è¯api[manga-image-translator](https://github.com/zyddnys/manga-
 image-translator),ç°å¨ä½ å¯ä»¥ä½éªæ¬å°çç¿»è¯ - 2023-04-28: -
 æä»¶åå¸ ## ð¦è®¡å - [x] ééç¦»çº¿ç¿»è¯æ¨¡å[manga-image-
 translator](https://github.com/zyddnys/manga-image-translator) - [x]
-æ¯ææ´å¤API - [ ] å®åæä»¶ ##
+æ¯ææ´å¤API - [x] å¤å¹³å°éé - [ ]
+æ¯ææå®æºè¯­è¨åç®æ è¯­è¨ - [ ] å®åæä»¶ ##
 â¨åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ï¼ççäºQAQ
```

