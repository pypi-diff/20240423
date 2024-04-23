# Comparing `tmp/sts_lib-0.26.0.tar.gz` & `tmp/sts_lib-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.26.0.tar", last modified: Thu Apr 18 15:53:22 2024, max compression
+gzip compressed data, was "sts_lib-0.27.0.tar", last modified: Tue Apr 23 04:16:18 2024, max compression
```

## Comparing `sts_lib-0.26.0.tar` & `sts_lib-0.27.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.094695 sts_lib-0.26.0/
--rw-rw-rw-   0        0        0    11358 2024-04-18 15:53:10.000000 sts_lib-0.26.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-18 15:53:10.000000 sts_lib-0.26.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7669 2024-04-18 15:53:22.093691 sts_lib-0.26.0/PKG-INFO
--rw-rw-rw-   0        0        0     6216 2024-04-18 15:53:10.000000 sts_lib-0.26.0/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-18 15:53:22.095690 sts_lib-0.26.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-18 15:53:10.000000 sts_lib-0.26.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.048737 sts_lib-0.26.0/sts/
--rw-rw-rw-   0        0        0    43558 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.049736 sts_lib-0.26.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.064741 sts_lib-0.26.0/sts/data/config/
--rw-rw-rw-   0        0        0      723 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      383 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      289 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      337 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      303 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      215 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      301 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      383 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      211 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      225 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      215 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      209 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      381 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      427 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      287 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.080705 sts_lib-0.26.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    21185 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.083701 sts_lib-0.26.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.091693 sts_lib-0.26.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     7669 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.045346 sts_lib-0.27.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10790 2024-04-23 04:16:18.044347 sts_lib-0.27.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9337 2024-04-23 04:11:40.000000 sts_lib-0.27.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-23 04:16:18.046345 sts_lib-0.27.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:17.999124 sts_lib-0.27.0/sts/
+-rw-rw-rw-   0        0        0    52284 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-23 03:16:40.000000 sts_lib-0.27.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.000104 sts_lib-0.27.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.014962 sts_lib-0.27.0/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.031403 sts_lib-0.27.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22760 2024-04-23 02:29:50.000000 sts_lib-0.27.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.035384 sts_lib-0.27.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.042349 sts_lib-0.27.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0    10790 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.26.0/LICENSE` & `sts_lib-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/PKG-INFO` & `sts_lib-0.27.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.26.0
+Version: 0.27.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -35,38 +35,46 @@
 
 # STS 簡繁祕書
 
 STS (Simplified-Traditional Secretary) is an open library for flexible simplified-traditional Chinese text conversion.
 
 簡繁祕書是開源、輕巧、有彈性的中文簡繁轉換工具，也支援異體字轉換及地區慣用詞轉換。
 
+
 ## Features 特色
 
-* 使用與 [OpenCC](https://github.com/BYVoid/OpenCC) 格式相容的詞典檔。
+* 使用與 [OpenCC](https://github.com/BYVoid/OpenCC) 格式相容的詞典檔。此外亦支援 JSON 或 YAML 格式的詞典檔。
 * 可「並聯」或「串聯」組合多個詞典檔作為轉換方案，並預先儲存成單一詞典檔以加速載入。詞典檔更新時也會自動重新生成組合詞典。
 * 簡繁對應、異體字對應、地區慣用詞對應等不同的對應關係皆區分至不同的詞典檔。
 * 詞典及配置檔與程式本體分離，可自由修改、擴充。
 * 支援一對多轉換，轉換結果可輸出為純文字、HTML、JSON 等格式。
 * 支援 Unicode 組合字，例如「⿰虫鬼」視為一個字，不會因為詞典有「虫=>蟲」而被轉為「⿰蟲鬼」。
 * 支援用正規表示式略過特定文字的轉換。
 * 支援編碼轉換，可自訂輸入及輸出檔案的字元編碼。
 
+
 ## Usage 使用
 
 ### Installation 安裝
 
+安裝 Python >= 3.7 ([官網](https://www.python.org/))，然後在命令列輸入以下指令安裝（或升級至）最新版本：
+
     pip install -U sts-lib
 
+> 若要支援 YAML 格式，須額外安裝 PyYAML 套件，或改用以下指令安裝：
+>
+>    pip install -U sts-lib[yaml]
+
 ### Command Line
 
 * `sts --help` 或 `sts COMMAND --help` 檢視可用指令的詳細說明文檔。
 
 * `sts convert [OPTIONs] [file ...]` 執行簡繁轉換：
   * `file` 為一或多個欲轉換的檔案。（省略則讀取標準輸入 STDIN）
-  * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
+  * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製配置檔（JSON 或 YAML）的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如可輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
   * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return`（或 `return1`, `return2`, ... 等）子群組時會取代為子群組的值。
@@ -96,54 +104,129 @@
                        input_encoding='UTF-8', output_encoding='UTF-8',
                        format='txt', exclude=None)
 
 # perform a conversion for a string and process the result data generator
 [p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
 ```
 
-## Config 配置檔
+
+## Advanced 進階開發
+
+### Config 配置檔
+
+配置檔為 JSON 或 YAML 檔案（副檔名須為 `.yaml` 或 `.yml`）。規格如下：
 
 ```javascript
 /**
  * @typedef {Object} configScheme
  * @property {string} [name] - name/description of the config
  * @property {string[]} [requires] - required configs, which are made before
  *     making from this config, as an absolute path, or a path relative to the
  *     directory of this config file, or the basename of a built-in config file
- *     (with or without ".json")
- * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
+ *     (with or without extension ".json", ".yaml", ".yml")
+ * @property {srcDictScheme[]} dicts - schemes of each dictionary file to be
+ *     generated or loaded.
+ */
+
+/**
+ * A dictScheme or string for a dict.
+ *
+ * The string should be an absolute path, or a path relative to the directory
+ * of the config file, or the basename of a built-in dictionary file, with a
+ * file extension of .txt, .list, .json, .jlist, .yaml, or .yml.
+ *
+ * @typedef {(string|dictScheme)} srcDictScheme
  */
 
 /**
  * @typedef {Object} dictScheme
- * @property {string} file - path of the dictionary file to generate, as an
+ * @property {string} [file] - path of the dictionary file to generate, as an
  *     absolute path, or a path relative to the directory of this config file.
  *     It should be a .tlist (compiled trie), .jlist (compiled table), or .list
- *     (plain text table).
- * @property {string} [mode=load] - the mode to handle the loaded source files:
- *     "load" to simply merge the loaded keys and values; "swap" to reverse the
- *     dictionary (i.e. use the values as keys and the keys as values); "join"
- *     to build from a chain of dictionaries (in which case src must be an
- *     array of subarrays of strings)
- * @property {Array.<(string|string[])>} [src] - the source files. Each as an
- *     absolute path, or a path relative to the directory of this config file,
- *     or the basename of a built-in dictionary file. Each should be a .txt,
- *     .list, .json, .jlist, .yaml, or .yml dictionary file. File must exist
- *     when this is omitted.
+ *     (plain text table). An unknown file extension is treated as .list. `src`
+ *     must exist when omitted.
+ * @property {string} [mode=load] - the mode to handle the loaded dicts.
+ *     - "load" to simply merge the loaded keys and values;
+ *     - "swap" to reverse the dict (i.e. use the values as keys and the keys
+ *       as values);
+ *     - "join" to chain dicts (a conversion using a dict joining dict1 and
+ *       dict2 works like a conversion using dict1 and then dict2, but takes
+ *       care of word segmentation);
+ *     - "filter" to filter the output values in the loaded dicts with extra
+ *       "include" and "exclude" properties
+ *     - "expand" to expand the placeholders (defined in the extra
+ *       "placeholders" property) in the first dict with the matching key and
+ *        value in other dicts;
+ *     - "remove_keys" to remove keys from the first dict if it appears in any
+ *       other one;
+ *     - "remove_values" to remove key-value pairs from the first dict if it
+ *       appears in any other one.
+ * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
+ *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
- * @property {string} [include] - a regex filter that discards non-matched
- *     conversion values.
- * @property {string} [exclude] - a regex filter that discards matched
- *     conversion values.
  * @property {boolean} [check] - true to raise an exception if the output
  *     contains an invalid char which will be loaded incorrectly. Set this
  *     when the output is a plain text table file and the source files contain
  *     untrusted JSON or YAML data that may include a char like " ", "\t",
  *     "\n", etc. in the dictionary.
+ * @property {string} [include] - a regex filter that discards non-matched
+ *     conversion values. (for "filter" mode)
+ * @property {string} [exclude] - a regex filter that discards matched
+ *     conversion values. (for "filter" mode)
+ * @property {string[]} [placeholders] - strings to be expanded using other
+ *     dicts. (for "expand" mode)
  */
 ```
 
+### Dictionary 詞典檔
+
+原始詞典檔可為純文字、JSON、或 YAML。規格如下：
+
+#### 純文字
+
+純文字詞典副檔名為 .txt。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
+
+```
+輸入詞1\t轉換詞11 轉換詞12 ...
+輸入詞2\t轉換詞21 轉換詞22 ...
+...
+```
+
+注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外也不可含有換行等字元。
+
+#### JSON
+
+JSON 詞典副檔名為 `.json`。規格如下：
+
+```
+{
+  "輸入詞1": ["轉換詞11", "轉換詞12", ...],
+  "輸入詞2": ["轉換詞22", "轉換詞22", ...],
+  ...
+}
+```
+
+#### YAML
+
+YAML 詞典副檔名為 `.yaml` 或 `.yml`。規格如下：
+
+```
+輸入詞1: [轉換詞11, 轉換詞12, ...]
+輸入詞2: [轉換詞22, 轉換詞22, ...]
+...
+```
+
+
+## 線上版
+
+[簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
+
+本線上轉換工具支援文字轉換及檔案轉換。前者只要在輸入區填入文字，就會自動轉換並且可以互動式校訂。後者可以用按鈕或拖放選擇一或多個檔案，就會逐一轉換後自動下載。預設檔案輸入輸出編碼皆是UTF-8，如要輸入其他編碼的檔案，可在進階選項設定。
+
+目前內建 [OpenCC](https://github.com/BYVoid/OpenCC)、[MediaWiki](https://github.com/wikimedia/mediawiki)、[新同文堂](https://github.com/tongwentang/tongwen-dict)的轉換方案，並且修正了 OpenCC 演算法缺陷導致一些地區詞無法正常轉換的問題（詳見[相關問題回報](https://github.com/BYVoid/OpenCC/issues/475)）。
+
+
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
 
 詞典檔原始資料來自同文堂、維基百科、OpenCC 等開源專案，再按本專案之需求編校。
```

### Comparing `sts_lib-0.26.0/setup.cfg` & `sts_lib-0.27.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/__init__.py` & `sts_lib-0.27.0/sts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.26.0'
+__version__ = '0.27.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -252,14 +252,19 @@
                 return False
             keys.add(key)
         for key in other:
             if key not in keys:
                 return False
         return True
 
+    def __delitem__(self, key):
+        """Implementation of del self[key].
+        """
+        del self._dict[key]
+
     def keys(self):
         """Get a generator of keys.
         """
         yield from self._dict.keys()
 
     def values(self):
         """Get a generator of values.
@@ -289,25 +294,23 @@
         Args:
             skip_check: True to skip checking duplicated values.
         """
         for key, values in stsdict.items():
             self.add(key, values, skip_check=skip_check)
         return self
 
-    def load(self, *files, type=None):
-        """Add all key-values pairs from dict file(s).
-        """
-        for file in files:
-            t = os.path.splitext(file)[1][1:].lower() if type is None else type
-            if t in ('json', 'jlist'):
-                self._load_json(file)
-            elif t in ('yaml', 'yml'):
-                self._load_yaml(file)
-            else:
-                self._load_plain(file)
+    def load(self, file, type=None):
+        """Add all key-values pairs from a dict file."""
+        t = os.path.splitext(file)[1][1:].lower() if type is None else type
+        if t in ('json', 'jlist'):
+            self._load_json(file)
+        elif t in ('yaml', 'yml'):
+            self._load_yaml(file)
+        else:
+            self._load_plain(file)
         return self
 
     def _load_plain(self, file):
         with open(file, 'r', encoding='UTF-8') as fh:
             for line in fh:
                 try:
                     key, values, *_ = line.rstrip('\n').split('\t')
@@ -362,24 +365,25 @@
                     for badchar in ' \t\n\r':
                         if any(badchar in v for v in values):
                             raise ValueError(
                                 f'{repr(key)} => {repr(values)} contains invalid {repr(badchar)}'
                             )
                 fh.write(f'{key}\t{" ".join(values)}\n')
 
-    def loadjson(self, file):
+    @classmethod
+    def loadjson(cls, file):
         """Load from a JSON file.
 
         NOTE: The input data format may vary across subclasses.
 
         Returns:
             a new object with the same class.
         """
         with open(file, 'r', encoding='UTF-8') as fh:
-            stsdict = self.__class__()
+            stsdict = cls()
             stsdict._dict = json.load(fh)
         return stsdict
 
     def dumpjson(self, file=None, indent=None, sort=False):
         """Dump key-values pairs to a JSON file.
 
         NOTE: The output data format may vary across subclasses.
@@ -797,14 +801,25 @@
         return sum(1 for _ in self)
 
     def __iter__(self):
         """Implementation of iter(self).
         """
         yield from self.keys()
 
+    def __delitem__(self, key):
+        """Implementation of del self[key].
+        """
+        trie = self._dict
+        try:
+            for k in self._split(key):
+                trie = trie[k]
+            del trie['']
+        except KeyError:
+            raise KeyError(key)
+
     def keys(self):
         """Get a generator of keys.
         """
         def recurse(trie):
             for key in trie:
                 if key == '':
                     yield ''.join(keystack)
@@ -920,20 +935,21 @@
                 ],
                 "dicts": [  // dictionaries to generate
                     {
                         "file": "...",  // path of the generated dictionary
                                         // file, relative to config dir
                         "mode": "...",  // mode to handle the loaded sources:
                                         // load, swap, join
-                        "src": ["...", ...]  // list of the source file paths,
-                                             // should be .txt or .list files
+                        "src": [        // list of the source file paths,
+                            src1,       // should be .txt or .list files
+                            src2,
+                            ...
+                        ],
                         "sort": true,   // truthy to sort the keys of the
                                         // generated dictionary
-                        "include": "...",  // regex filter for output values
-                        "exclude": "...",  // regex filter for output values
                         "check": true,  // check for invalid output
                     },
                     ...
                 ]
             }
 
         Args:
@@ -947,95 +963,335 @@
 
         Returns:
             a str for the path of the last generated dictionary file
         """
         # locate and load the config file
         config_file = self.get_config_file(config_name, base_dir=base_dir)
         config_dir = os.path.abspath(os.path.dirname(config_file))
-
-        with open(config_file, 'r', encoding='UTF-8') as fh:
-            config = json.load(fh)
+        config = self.load_config(config_file)
+        self.normalize_config(config, config_dir)
 
         # handle required configs
         if not skip_requires:
-            for cf in config.get('requires', []):
+            for cf in config['requires']:
                 self.make(cf, base_dir=config_dir, skip_requires=skip_requires, quiet=quiet)
 
         # make the requested dicts
-        for dict_ in config['dicts']:
-            dest = os.path.normpath(os.path.join(config_dir, dict_['file']))
-            format = os.path.splitext(dest)[1][1:].lower()
-            mode = dict_.get('mode', 'load')
-            src = dict_.get('src', [])
-            sort = dict_.get('sort', False)
-            include = dict_.get('include', None)
-            exclude = dict_.get('exclude', None)
-            check = dict_.get('check', False)
-
-            files = self.resolve_src_files(src, config_dir)
+        for dict_scheme in config['dicts']:
+            if isinstance(dict_scheme, str):
+                dest = dict_scheme
+                if not os.path.isfile(dest):
+                    raise RuntimeError(f'specified dict file does not exist: {dest}')
+                continue
 
-            if include is not None:
-                try:
-                    include = re.compile(include)
-                except re.error as exc:
-                    raise ValueError(f'regex syntax error of the include filter: {exc}')
+            dest = dict_scheme['file']
 
-            if exclude is not None:
-                try:
-                    exclude = re.compile(exclude)
-                except re.error as exc:
-                    raise ValueError(f'regex syntax error of the exclude filter: {exc}')
-
-            if not files:
-                if os.path.isfile(dest):
-                    if not quiet:
-                        print(f'skip making (no src): {dest}')
-                    continue
-                else:
-                    raise RuntimeError(f'Specified flie does not exist: {dest}')
+            if dest is None:
+                raise RuntimeError('dict["file"] is not specified')
 
-            if not skip_check and not self.check_update(dest, files):
+            if not skip_check and not self.check_update(dict_scheme):
                 if not quiet:
                     print(f'skip making (up-to-date): {dest}')
                 continue
 
-            if not quiet:
-                print(f'making: {dest}')
+            self.make_dict(dict_scheme, config_dir=config_dir, skip_check=skip_check, quiet=quiet)
 
-            if mode == 'load':
-                table = Table().load(*files)
-            elif mode == 'swap':
-                table = Table().load(*files).swap()
-            elif mode == 'join':
-                table = Table()
-                for dict_ in (Table().load(*fg) for fg in files):
-                    table = table.join(dict_)
-            else:
-                raise ValueError(f'Specified mode is not supported: {mode}')
+        return dest
 
-            if include is not None or exclude is not None:
-                _table = table
-                table = Table()
-                for key, values in _table.items():
-                    values = [v for v in values
-                              if (include is None or include.search(v))
-                              and (exclude is None or not exclude.search(v))]
-                    if values:
-                        table.add(key, values)
+    def load_config(self, config_file):
+        ext = os.path.splitext(config_file)[1][1:].lower()
 
-            os.makedirs(os.path.dirname(dest), exist_ok=True)
+        if ext in ('yaml', 'yml'):
+            try:
+                import yaml
+            except ModuleNotFoundError:
+                raise RuntimeError('install PyYAML module to support loading .yaml config')
+
+            with open(config_file, 'r', encoding='UTF-8') as fh:
+                config = yaml.safe_load(fh)
+
+        else:  # default: json
+            with open(config_file, 'r', encoding='UTF-8') as fh:
+                config = json.load(fh)
+
+        return config
+
+    def normalize_config(self, config, config_dir):
+        """Normalize and validate config in place."""
+        if not isinstance(config, dict):
+            raise ValueError('config is not a dict')
+
+        config.setdefault('requires', [])
+
+        try:
+            dict_schemes = config['dicts']
+        except KeyError:
+            raise ValueError('config["dicts"] is not specified')
+
+        for i, dict_scheme in enumerate(dict_schemes):
+            dict_schemes[i] = self.normalize_dict_scheme(dict_scheme, config_dir)
+
+        return config
+
+    def normalize_dict_scheme(self, dict_scheme, config_dir):
+        """Recursively normalize and validiate dict_scheme in place.
+
+        - Resolve file paths.
+
+        Args:
+            dict_scheme: a dict or a str for the dictionary path
+        """
+        if isinstance(dict_scheme, str):
+            return self.get_stsdict_file(dict_scheme, config_dir)
+
+        try:
+            dict_scheme['file'] = os.path.normpath(os.path.join(config_dir, dict_scheme['file']))
+        except KeyError:
+            dict_scheme['file'] = None
+
+        try:
+            srcs = dict_scheme['src']
+        except KeyError:
+            dict_scheme['src'] = []
+        else:
+            for i, src in enumerate(srcs):
+                srcs[i] = self.normalize_dict_scheme(src, config_dir)
+
+        mode = dict_scheme.setdefault('mode', 'load')
+        dict_scheme['sort'] = bool(dict_scheme.get('sort'))
+        dict_scheme['check'] = bool(dict_scheme.get('check'))
+
+        if mode == 'filter':
+            try:
+                dict_scheme['include'] = re.compile(dict_scheme['include'])
+            except KeyError:
+                dict_scheme['include'] = None
+            except re.error as exc:
+                raise ValueError(f'regex syntax error of the "include" filter: {exc}')
+
+            try:
+                dict_scheme['exclude'] = re.compile(dict_scheme['exclude'])
+            except KeyError:
+                dict_scheme['exclude'] = None
+            except re.error as exc:
+                raise ValueError(f'regex syntax error of the "exclude" filter: {exc}')
+
+        elif mode == 'expand':
+            dict_scheme.setdefault('placeholders', [])
+            if len(dict_scheme['placeholders']) != len(srcs) - 1:
+                raise ValueError('length of dict["placeholders"] does not match dict["src"]')
+
+        return dict_scheme
+
+    def make_dict(self, dict_scheme, config_dir, skip_check=False, quiet=False):
+        """Make a dict.
 
+        Returns:
+            A StsDict or str (for str scheme or when up-to-date).
+        """
+        if isinstance(dict_scheme, str):
+            return dict_scheme
+
+        dest = dict_scheme.get('file')
+        if dest:
+            if not dict_scheme.get('_updated'):
+                return dest
+
+            format = os.path.splitext(dest)[1][1:].lower()
+        else:
+            format = '.list'
+
+        mode = dict_scheme['mode']
+        srcs = dict_scheme['src']
+        sort = dict_scheme['sort']
+
+        if not srcs:
+            if not os.path.isfile(dest):
+                raise RuntimeError(f'Specified flie does not exist: {dest}')
+            return dest
+
+        if dest and not quiet:
+            print(f'making: {dest}')
+
+        for i, src in enumerate(srcs):
+            srcs[i] = self.make_dict(src, config_dir, skip_check, quiet)
+
+        try:
+            func = getattr(self, f'_make_dict_mode_{mode}')
+        except AttributeError:
+            raise ValueError(f'Specified mode is not supported: {mode}')
+        else:
+            table = func(dict_scheme)
+
+        if dest:
+            os.makedirs(os.path.dirname(dest), exist_ok=True)
             if format == 'tlist':
                 Trie(table).dumpjson(dest, sort=sort)
             elif format == 'jlist':
                 table.dumpjson(dest, sort=sort)
             else:  # default: list
-                table.dump(dest, sort=sort, check=check)
+                table.dump(dest, sort=sort, check=dict_scheme['check'])
 
-        return dest
+        return table
+
+    def _make_dict_mode_load(self, dict_scheme):
+        table = Table()
+        for src in dict_scheme['src']:
+            if isinstance(src, str):
+                table.load(src)
+            else:
+                for key, values in src.items():
+                    table.add(key, values)
+        return table
+
+    def _make_dict_mode_filter(self, dict_scheme):
+        table = self._make_dict_mode_load(dict_scheme)
+
+        include = dict_scheme['include']
+        exclude = dict_scheme['exclude']
+        if include or exclude:
+            _table = table
+            table = Table()
+            for key, values in _table.items():
+                values = [v for v in values
+                          if (include is None or include.search(v))
+                          and (exclude is None or not exclude.search(v))]
+                if values:
+                    table.add(key, values)
+
+        return table
+
+    def _make_dict_mode_swap(self, dict_scheme):
+        table = self._make_dict_mode_load(dict_scheme)
+        table = table.swap()
+        return table
+
+    def _make_dict_mode_join(self, dict_scheme):
+        table = Table()
+        for src in dict_scheme['src']:
+            dict_ = Table().load(src) if isinstance(src, str) else src
+            table = table.join(dict_)
+        return table
+
+    def _make_dict_mode_expand(self, dict_scheme):
+        newtable = Table()
+
+        srcs = dict_scheme['src']
+        src = srcs.pop(0)
+        table = Table().load(src) if isinstance(src, str) else src
+        dicts = [Table().load(src) if isinstance(src, str) else src for src in srcs]
+
+        placeholders = dict_scheme['placeholders']
+        placeholders_re = re.compile('|'.join(re.escape(p) for p in placeholders))
+        map_placeholder_to_idx = {p: i for i, p in enumerate(placeholders)}
+
+        for key, values in table.items():
+            key_parts = list(self._make_dict_mode_expand_split(key, placeholders_re))
+            value_parts_list = [list(self._make_dict_mode_expand_split(v, placeholders_re)) for v in values]
+
+            map_placeholder_to_dict_keys = {}
+            for part in itertools.chain(key_parts, *value_parts_list):
+                if isinstance(part, str):
+                    continue
+                key = part[0]
+                key_idx = map_placeholder_to_idx[key]
+                dict_keys = dicts[key_idx].keys()
+                map_placeholder_to_dict_keys[key] = dict_keys
+
+            for comb in itertools.product(*map_placeholder_to_dict_keys.values()):
+                newkey = self._make_dict_mode_expand_get_expanded_key(key_parts, comb, map_placeholder_to_idx)
+                newvalues = [
+                    self._make_dict_mode_expand_get_expanded_value(vpp, comb, map_placeholder_to_idx, dicts)
+                    for vpp in value_parts_list
+                ]
+                newtable.add(newkey, newvalues)
+
+        return newtable
+
+    @staticmethod
+    def _make_dict_mode_expand_split(text, placeholders_re):
+        index = 0
+        for m in placeholders_re.finditer(text):
+            start, end = m.span(0)
+
+            t = text[index:start]
+            if t:
+                yield t
+
+            t = m.group(0)
+            if t:
+                yield (t,)
+
+            index = end
+
+        t = text[index:]
+        if t:
+            yield t
+
+    @staticmethod
+    def _make_dict_mode_expand_get_expanded_key(parts, comb, map_placeholder_to_idx):
+        rv = []
+        for part in parts:
+            if isinstance(part, str):
+                rv.append(part)
+                continue
+
+            key = part[0]
+            key_idx = map_placeholder_to_idx[key]
+            rv.append(comb[key_idx])
+        return ''.join(rv)
+
+    @staticmethod
+    def _make_dict_mode_expand_get_expanded_value(parts, comb, map_placeholder_to_idx, dicts):
+        rv = []
+        for part in parts:
+            if isinstance(part, str):
+                rv.append(part)
+                continue
+
+            key = part[0]
+            key_idx = map_placeholder_to_idx[key]
+            try:
+                rv.append(dicts[key_idx][comb[key_idx]][0])
+            except IndexError:
+                rv.append(key)
+        return ''.join(rv)
+
+    def _make_dict_mode_remove_keys(self, dict_scheme):
+        srcs = dict_scheme['src']
+        src = srcs.pop(0)
+        table = Table().load(src) if isinstance(src, str) else src
+        for src in srcs:
+            dict_ = Table().load(src) if isinstance(src, str) else src
+            for k in dict_:
+                try:
+                    del table[k]
+                except KeyError:
+                    continue
+        return table
+
+    def _make_dict_mode_remove_values(self, dict_scheme):
+        srcs = dict_scheme['src']
+        src = srcs.pop(0)
+        table = Table().load(src) if isinstance(src, str) else src
+        for src in srcs:
+            dict_ = Table().load(src) if isinstance(src, str) else src
+            for k, vv in dict_.items():
+                try:
+                    t = table[k]
+                except KeyError:
+                    continue
+                for v in vv:
+                    try:
+                        t.remove(v)
+                    except ValueError:
+                        pass
+                if not t:
+                    del table[k]
+        return table
 
     def get_config_file(self, config, base_dir=None):
         """Calculate the path of a config file.
 
         1. Use it if it's an absolute path.
         2. Assume relative to base_dir or CWD.
         3. Assume relative to default config directory. (basename only; .json omissible)
@@ -1048,18 +1304,22 @@
         if os.path.isfile(relative_config):
             return os.path.normpath(relative_config)
 
         if os.path.basename(config) == config:
             search_file = os.path.join(self.config_dir, config)
             if os.path.isfile(search_file):
                 return os.path.normpath(search_file)
-            if not config.lower().endswith('.json'):
-                search_file = os.path.join(self.config_dir, config + '.json')
-                if os.path.isfile(search_file):
-                    return os.path.normpath(search_file)
+
+            exts = ('.json', '.yaml', '.yml')
+            ext = os.path.splitext(config)[1].lower()
+            if ext not in exts:
+                for ext in exts:
+                    search_file = os.path.join(self.config_dir, config + ext)
+                    if os.path.isfile(search_file):
+                        return os.path.normpath(search_file)
 
         return os.path.normpath(relative_config)
 
     def get_stsdict_file(self, stsdict, base_dir=None):
         """Calculate the path of a dictionary file.
 
         1. Use it if it's an absolute path.
@@ -1077,34 +1337,46 @@
         if os.path.basename(stsdict) == stsdict:
             search_file = os.path.join(self.dictionary_dir, stsdict)
             if os.path.isfile(search_file):
                 return os.path.normpath(search_file)
 
         return os.path.normpath(relative_stsdict)
 
-    def resolve_src_files(self, files, base_dir):
-        return [self.get_stsdict_file(f, base_dir=base_dir)
-                if isinstance(f, str)
-                else self.resolve_src_files(f, base_dir=base_dir)
-                for f in files]
+    def check_update(self, dict_scheme, mtime=math.inf):
+        """Recursively check if dict_scheme needs update.
 
-    def check_update(self, output, filegroups):
-        """Check if the output file needs update.
+        Updated dict_scheme or descendant dict_scheme sets
+        dict_scheme['_updated'] = True.
+
+        Returns:
+            bool: True if needs update and False otherwise.
         """
-        if not os.path.isfile(output):
-            return True
+        if isinstance(dict_scheme, str):
+            dict_scheme = {'file': dict_scheme}
 
-        for files in filegroups:
-            if isinstance(files, str):
-                files = [files]
-            for file in files:
-                if os.path.getmtime(file) > os.path.getmtime(output):
-                    return True
+        rv = False
+
+        file = dict_scheme.get('file')
+
+        if file:
+            if not os.path.isfile(file):
+                rv = dict_scheme['_updated'] = True
+            else:
+                file_mtime = os.path.getmtime(file)
+                if file_mtime > mtime:
+                    rv = True
+
+                mtime = file_mtime
+
+        srcs = dict_scheme.get('src', ())
+        for src in srcs:
+            if self.check_update(src, mtime):
+                rv = dict_scheme['_updated'] = True
 
-        return False
+        return rv
 
 
 class StsConverter():
     """Convert a text using an stsdict.
     """
     exclude_return_group_pattern = re.compile(r'^return\d*$')
     template_placeholder_pattern = re.compile(r'%(\w*)%')
@@ -1118,17 +1390,17 @@
                 dictionary file
         """
         if isinstance(stsdict, StsDict):
             self.table = stsdict
         else:
             _, ext = os.path.splitext(stsdict)
             if ext.lower() == '.jlist':
-                self.table = Table().loadjson(stsdict)
+                self.table = Table.loadjson(stsdict)
             elif ext.lower() == '.tlist':
-                self.table = Trie().loadjson(stsdict)
+                self.table = Trie.loadjson(stsdict)
             else:  # default: list
                 self.table = Table().load(stsdict)
 
     def convert(self, text, exclude=None):
         """Convert a text and yield each part.
 
         Yields:
```

### Comparing `sts_lib-0.26.0/sts/cli.py` & `sts_lib-0.27.0/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/config/_default.json` & `sts_lib-0.27.0/sts/data/config/hk2s.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35000000000000003%*

 * *Differences: {"'dicts'": "{0: {'file': '../dictionary/hk2s.tlist', 'mode': 'join', 'src': "*

 * *            "[OrderedDict([('mode', 'load'), ('src', ['../dictionary/HKVariantsRevPhrases.txt', "*

 * *            "'../dictionary/HKVariantsRev.list'])]), OrderedDict([('mode', 'load'), ('src', "*

 * *            "['../dictionary/TSPhrases.txt', '../dictionary/TSCharacters.txt'])])]}, delete: [3, "*

 * *            '2, 1, 0]}',*

 * * "'name'": "'Traditional Chinese (Hong Kong variant) to Simplified Chinese'",*

 * * "'requires'": "['_default.json']"}*

```diff
@@ -1,42 +1,28 @@
 {
     "dicts": [
         {
-            "file": "../dictionary/TWPhrases.list",
-            "mode": "load",
+            "file": "../dictionary/hk2s.tlist",
+            "mode": "join",
             "src": [
-                "TWPhrasesIT.txt",
-                "TWPhrasesName.txt",
-                "TWPhrasesOther.txt"
-            ]
-        },
-        {
-            "file": "../dictionary/TWPhrasesRev.list",
-            "mode": "swap",
-            "src": [
-                "TWPhrases.list"
-            ]
-        },
-        {
-            "file": "../dictionary/TWVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "TWVariants.txt"
-            ]
-        },
-        {
-            "file": "../dictionary/HKVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "HKVariants.txt"
-            ]
-        },
-        {
-            "file": "../dictionary/JPVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "JPVariants.txt"
+                {
+                    "mode": "load",
+                    "src": [
+                        "../dictionary/HKVariantsRevPhrases.txt",
+                        "../dictionary/HKVariantsRev.list"
+                    ]
+                },
+                {
+                    "mode": "load",
+                    "src": [
+                        "../dictionary/TSPhrases.txt",
+                        "../dictionary/TSCharacters.txt"
+                    ]
+                }
             ]
         }
     ],
-    "name": "Built-in dictionaries"
+    "name": "Traditional Chinese (Hong Kong variant) to Simplified Chinese",
+    "requires": [
+        "_default.json"
+    ]
 }
```

### Comparing `sts_lib-0.26.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.27.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.27.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.27.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.27.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.27.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.27.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.27.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.27.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.27.0/sts/data/htmlpage.tpl.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 <!DOCTYPE html>
-<html>
+<html lang="zh-Hant">
 <head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width">
 <title>簡繁祕書 v%VERSION%</title>
 <style>
 kbd { border: 1px solid #999; border-radius: 2px; padding: 2px 4px; background-color: #f5f5f5; font-weight: bold; }
+dialog:not([open]) { display: none; }
 dialog header { margin-bottom: .5em; font-weight: bold; }
 dialog section { margin: .5em 0; }
 dialog section label { display: block; }
 dialog footer { margin-top: 1em; display: flex; gap: .5em 1em; flex-direction: row; flex-wrap: wrap; }
 dialog footer input { flex-grow: 1; }
 body > footer { margin-top: 1em; text-align: center; font-size: small; }
 #viewer { border: thin ridge #0066CC; padding: 0.5em; background-color: #f8f8ee; white-space: pre-wrap; }
 #viewer a { border: thin dotted #AAA; color: unset; text-decoration: none; }
 #viewer a:focus { outline: medium solid blue; }
 #viewer a.single, .single { background-color: #DDDDDD; }  /* 單選字 */
+#viewer a.changed, .changed { background-color: #DDDDFF; }  /* 異動字 */
 #viewer a.unchecked, .unchecked { background-color: #FFFF99; }  /* 未審字 */
 #viewer a.checked, .checked { background-color: #CCFFFF; }  /* 已審字 */
 #viewer a.picked, .picked { background-color: #CCFFCC; }  /* 選定字 */
 #viewer a.editing, .editing { background-color: #FFDDDD; }  /* 編輯中 */
 #viewer a ins, #viewer a del { text-decoration: none; }
 .popup {
   position: absolute;
@@ -35,44 +37,60 @@
   align-items: center;
 }
 .popup a { padding: .3em; cursor: pointer; }
 .popup a:hover { background-color: #ccc; }
 .popup a:not([tabindex="0"])::before { content: attr(tabindex) "."; }
 </style>
 <script>
-function moveAnchor(anchor, offset, filter) {
-  const viewer = document.querySelector('#viewer');
-  const anchors = viewer.querySelectorAll('a');
-  const len = anchors.length;
-
-  // no anchor, it's impossible to move
-  if (len === 0) {
-    return false;
+function* walkThroughAnchors(anchor, direction) {
+  let a = anchor;
+  if (direction > 0) {
+    while (a = a.nextElementSibling) {
+      if (a === anchor) { return; }
+      yield a;
+    }
+    if (a = anchor.parentNode.firstElementChild) {
+      if (a === anchor) { return; }
+      yield a;
+      while (a = a.nextElementSibling) {
+        if (a === anchor) { return; }
+        yield a;
+      }
+    }
+    return;
   }
-
-  let idx = Array.prototype.indexOf.call(anchors, anchor);
-
-  if (idx === -1) {
-    throw new Error(`specified anchor is invalid`);
+  if (direction < 0) {
+    while (a = a.previousElementSibling) {
+      if (a === anchor) { return; }
+      yield a;
+    }
+    if (a = anchor.parentNode.lastElementChild) {
+      if (a === anchor) { return; }
+      yield a;
+      while (a = a.previousElementSibling) {
+        if (a === anchor) { return; }
+        yield a;
+      }
+    }
+    return;
   }
+}
 
-  let anchorNew;
-  while (true) {
-    idx += offset;
-    while (idx >= len) { idx -= len; }
-    while (idx < 0) { idx += len; }
-    anchorNew = anchors[idx];
-    if (anchorNew === anchor) {
-      return false;
-    }
-    if (typeof filter !== "function" || filter(anchorNew)) {
-      break;
+function moveAnchor(anchor, offset, filter) {
+  let i = Math.abs(offset);
+  for (const a of walkThroughAnchors(anchor, offset)) {
+    if (typeof filter !== "function" || filter(a)) {
+      if (i > 1) {
+        i--;
+        continue;
+      }
+      return a;
     }
   }
-  return anchorNew;
+  return null;
 }
 
 function moveCandidate(anchor, offset, filter) {
   const cands = anchor.querySelectorAll('ins');
   const len = cands.length;
 
   // no cand, it's impossible to move
@@ -267,14 +285,24 @@
   });
   if (!anchorNew) {
     return;
   }
   anchorNew.focus();
 }
 
+function moveToChanged(anchor, offset) {
+  const anchorNew = moveAnchor(anchor, offset, a => {
+    return a.matches('.changed');
+  });
+  if (!anchorNew) {
+    return;
+  }
+  anchorNew.focus();
+}
+
 function moveToAny(anchor, offset) {
   const anchorNew = moveAnchor(anchor, offset);
   if (!anchorNew) {
     return;
   }
   anchorNew.focus();
 }
@@ -360,14 +388,16 @@
   const cmds = {
     "moveToUncheckedBackward": "移至上一個未審字",
     "moveToUncheckedForward": "移至下一個未審字",
     "moveToCheckworthyBackward": "移至上一個待校字",
     "moveToCheckworthyForward": "移至下一個待校字",
     "moveToSameBackward": "移至上一個相同字",
     "moveToSameForward": "移至下一個相同字",
+    "moveToChangedBackward": "移至上一個異動字",
+    "moveToChangedForward": "移至下一個異動字",
     "moveToAnyBackward": "移至上一個字",
     "moveToAnyForward": "移至下一個字",
 
     "applyBackwardUnchecked": "將目前選字套用至前面所有未審的相同字",
     "applyForwardUnchecked": "將目前選字套用至後面所有未審的相同字",
     "applyAllUnchecked": "將目前選字套用至全文所有未審的相同字",
     "applyBackward": "將目前選字套用至前面所有相同字",
@@ -379,54 +409,45 @@
 
     "toggleEditing": "編輯文字",
     "editContext": "編輯前後文字",
   };
 
   if (typeof cmd === 'undefined') {
     if (typeof HTMLDialogElement !== 'undefined') {
-      const dialog = document.createElement('dialog');
-      const form = dialog.appendChild(document.createElement('form'));
-      form.method = 'dialog';
-      const header = form.appendChild(document.createElement('header'));
-      header.textContent = '請選擇要執行的指令：';
-      const section = form.appendChild(document.createElement('section'));
-      const footer = form.appendChild(document.createElement('footer'));
-      const submitBtn = footer.appendChild(document.createElement('input'));
-      submitBtn.type = 'submit';
-      submitBtn.value = '確認';
-      const cancelBtn = footer.appendChild(document.createElement('input'));
-      cancelBtn.type = 'button';
-      cancelBtn.value = '取消';
-      cancelBtn.addEventListener('click', (event) => {
-        dialog.close('');
-      });
-      for (const cmd in cmds) {
-        const label = section.appendChild(document.createElement('label'));
-        const input = label.appendChild(document.createElement('input'));
-        input.type = 'radio';
-        input.name = 'cmd';
-        input.value = cmd;
-        label.appendChild(document.createTextNode(cmds[cmd]));
+      const dialog = document.getElementById('viewer-options');
+      const section = dialog.querySelector('form section');
+
+      // init options for commands for the first time
+      if (!section.children.length) {
+        for (const cmd in cmds) {
+          const label = section.appendChild(document.createElement('label'));
+          const input = label.appendChild(document.createElement('input'));
+          input.type = 'radio';
+          input.name = 'cmd';
+          input.value = cmd;
+          label.appendChild(document.createTextNode(cmds[cmd]));
+        }
+        section.querySelector('input').checked = true;
       }
 
-      const target = runCommand.lastCmd ?
-          section.querySelector(`input[value="${CSS.escape(runCommand.lastCmd)}"]`) :
-          section.querySelector('input');
-      target.checked = true;
-      target.autofocus = true;
+      // reset autofocus to the currently checked element
+      for (const elem of section.querySelectorAll('[autofocus]')) {
+        elem.autofocus = false;
+      }
+      section.querySelector(':checked').autofocus = true;
 
       cmd = await new Promise((resolve, reject) => {
-        dialog.addEventListener('close', (event) => {
+        function onClose(event) {
+          dialog.removeEventListener('close', onClose);
           const rv = dialog.returnValue ? dialog.querySelector('form').cmd.value : null;
           resolve(rv);
-        });
-        document.body.appendChild(dialog);
+        }
+        dialog.addEventListener('close', onClose);
         dialog.showModal();
       });
-      dialog.remove();
     } else {
       const idxMap = Array.from(Object.keys(cmds));
       const options = idxMap.map((cmd, i) => `${i + 1}.${cmds[cmd]}`);
       const msg = "請輸入要執行的指令：\n" + options.join('\n');
       const idx = parseInt(prompt(msg), 10);
       cmd = idxMap[idx - 1];
     }
@@ -451,14 +472,20 @@
       break;
     case "moveToSameBackward":
       moveToSame(anchor, -1);
       break;
     case "moveToSameForward":
       moveToSame(anchor, 1);
       break;
+    case "moveToChangedBackward":
+      moveToChanged(anchor, -1);
+      break;
+    case "moveToChangedForward":
+      moveToChanged(anchor, 1);
+      break;
     case "moveToAnyBackward":
       moveToAny(anchor, -1);
       break;
     case "moveToAnyForward":
       moveToAny(anchor, 1);
       break;
     case "applyBackwardUnchecked":
@@ -478,16 +505,14 @@
     case "toggleEditing":
       toggleEditing(anchor);
       break;
     case "editContext":
       editContext(anchor);
       break;
   }
-
-  runCommand.lastCmd = cmd;
 }
 
 function showPopup(anchor) {
   const popup = document.createElement('aside');
 
   const onMouseDown = (event) => {
     if (event.button !== 0) {
@@ -569,22 +594,37 @@
   return offset;
 }
 
 function onKeyDown(event) {
   const target = event.target.closest('a');
   if (!target) { return; }
 
-  if (target.matches('.editing') && event.key !== "`") {
+  // special combinations
+  if (event.shiftKey && event.key === "~" && !target.matches('.editing')) {
+    event.preventDefault();
+    editContext(target);
     return;
   }
 
   if (event.shiftKey || event.ctrlKey || event.altKey || event.metaKey) {
     return;
   }
 
+  if (target.matches('.editing')) {
+    switch (event.key) {
+      case "`":
+      case "Escape": {
+        event.preventDefault();
+        toggleEditing(target);
+        break;
+      }
+    }
+    return;
+  }
+
   switch (event.key) {
     case "`": {
       event.preventDefault();
       toggleEditing(target);
       break;
     }
     case "q": case "e": {
@@ -630,14 +670,21 @@
     }
   }
 }
 
 function onFocus(event) {
   const target = event.target.closest('a');
   if (!target) { return; }
+
+  // remove popup when editing
+  if (target.matches('.editing')) {
+    removePopup();
+    return;
+  }
+
   markChecked(target);
   removePopup();
   showPopup(target);
 }
 
 function onBlur(event) {
   const target = event.target.closest('a');
@@ -654,48 +701,66 @@
   for (const elem of viewer.querySelectorAll('a')) {
     elem.tabIndex = 0;
     const atomic = elem.hasAttribute('atomic');
     if (atomic) {
       elem.removeAttribute('atomic');
       elem.classList.add('atomic');
     }
-    const cls = (atomic && elem.querySelectorAll('ins').length <= 1) ? 'single' : 'unchecked';
+    const insElems = elem.querySelectorAll('ins');
+    const cls = (atomic && insElems.length <= 1) ? 'single' : 'unchecked';
     elem.classList.add(cls);
+    if (insElems[0] && elem.querySelector('del').textContent !== insElems[0].textContent) {
+      elem.classList.add('changed');
+    }
   }
 
   const target = viewer.querySelector('a.unchecked');
   if (target) { target.focus(); }
 });
 </script>
 </head>
 <body>
 <pre id="viewer">
 %CONTENT%</pre>
+<dialog id="viewer-options">
+<form method="dialog">
+  <header>請選擇要執行的指令：</header>
+  <section></section>
+  <footer>
+    <input type="submit" value="確認">
+    <input type="button" value="取消" onclick="this.closest('dialog').close('');">
+  </footer>
+</form>
+</dialog>
 <details>
 <summary>操作說明</summary>
 <p>使用滑鼠或以下操作鍵校對及處理文本，完成後可直接複製文本至他處使用。</p>
-<p>如果游標跑掉、操作鍵按了沒有反應，請點擊或用 <kbd>Tab</kbd> 鍵選擇任意上色標示的字，即可繼續用操作鍵操作。</p>
+<p>如果游標跑掉、操作鍵按了沒有反應，請用滑鼠或 <kbd>Tab</kbd> 鍵選擇任意上色標示的字，即可繼續用操作鍵操作。</p>
 
 <h3>上色標示說明</h3>
 <ul>
   <li><span class="single">灰色</span>：單選字。只有單一選項的字。</li>
+  <li><span class="changed">紫色</span>：異動字。轉換後與轉換前不同的字。</li>
   <li><span class="unchecked">黃色</span>：未審字。未檢查的字。</li>
   <li><span class="checked">藍色</span>：已審字。已檢查的字（未修改）。</li>
   <li><span class="picked">綠色</span>：已選字。已修改的字。</li>
   <li><span class="editing">紅色</span>：編輯中。可按 <kbd>`</kbd> 切換編輯模式。</li>
 </ul>
 
 <h3>操作鍵</h3>
 <ul>
   <li><kbd>Shift</kbd>+<kbd>Tab</kbd>／<kbd>Tab</kbd>：移至上／下一個字或欄位。</li>
   <li><kbd>Q</kbd>／<kbd>E</kbd>：移至上／下一個未審字。</li>
   <li><kbd>A</kbd>／<kbd>D</kbd>：移至上／下一個待校字（非單選字）。</li>
   <li><kbd>Z</kbd>／<kbd>C</kbd>：移至上／下一個相同字。</li>
   <li><kbd>W</kbd>／<kbd>S</kbd>：套用前／後一個候選字。</li>
   <li><kbd>0</kbd>-<kbd>9</kbd>：套用對應的候選字（<kbd>0</kbd>對應轉換前的字）。</li>
-  <li><kbd>`</kbd> (<kbd>1</kbd>左邊的反引號)：將此字切換為編輯模式，編輯模式下本鍵以外的操作鍵將無效。</li>
+  <li><kbd title='"1"左邊的反引號'>`</kbd>：將此字切換為編輯模式，可自由編輯。編輯模式下可用此鍵或<kbd>Esc</kbd>關閉編輯模式，其餘操作鍵無效。</li>
+  <li><kbd>Shift</kbd>+<kbd>`</kbd>：將前後未轉換文字切換為可點選操作。</li>
   <li><kbd>Enter</kbd>：開啟選單執行指令。</li>
 </ul>
 </details>
-<footer>Generated with <a href="https://pypi.org/project/sts-lib/">STS (Simplified-Traditional Secretary)</a> v%VERSION%. Released under <a href="http://www.apache.org/licenses/LICENSE-2.0">Apache License 2.0</a>.</footer>
+<footer>
+Generated with <a href="https://pypi.org/project/sts-lib/">STS (Simplified-Traditional Secretary)</a> v%VERSION%. Released under <a href="http://www.apache.org/licenses/LICENSE-2.0">Apache License 2.0</a>.
+</footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,21 +1,24 @@
 %CONTENT%
+請選擇要執行的指令：[??????????][Unknown INPUT type]
 操作說明
 使用滑鼠或以下操作鍵校對及處理文本，完成後可直接複製文本至他處使用。
-如果游標跑掉、操作鍵按了沒有反應，請點擊或用 Tab 鍵選擇任意上色標示的字，即可繼續用操作鍵操作。
+如果游標跑掉、操作鍵按了沒有反應，請用滑鼠或 Tab 鍵選擇任意上色標示的字，即可繼續用操作鍵操作。
 ******** ?上?色?標?示?說?明 ********
     * 灰色：單選字。只有單一選項的字。
+    * 紫色：異動字。轉換後與轉換前不同的字。
     * 黃色：未審字。未檢查的字。
     * 藍色：已審字。已檢查的字（未修改）。
     * 綠色：已選字。已修改的字。
     * 紅色：編輯中。可按 ` 切換編輯模式。
 ******** ?操?作?鍵 ********
     * Shift+Tab／Tab：移至上／下一個字或欄位。
     * Q／E：移至上／下一個未審字。
     * A／D：移至上／下一個待校字（非單選字）。
     * Z／C：移至上／下一個相同字。
     * W／S：套用前／後一個候選字。
     * 0-9：套用對應的候選字（0對應轉換前的字）。
-    * ` (1左邊的反引號)：將此字切換為編輯模式，編輯模式下本鍵以外的操作鍵將無效。
+    * `：將此字切換為編輯模式，可自由編輯。編輯模式下可用此鍵或Esc關閉編輯模式，其餘操作鍵無效。
+    * Shift+`：將前後未轉換文字切換為可點選操作。
     * Enter：開啟選單執行指令。
 Generated with _S_T_S_ _(_S_i_m_p_l_i_f_i_e_d_-_T_r_a_d_i_t_i_o_n_a_l_ _S_e_c_r_e_t_a_r_y_) v%VERSION%. Released
 under _A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0.
```

### Comparing `sts_lib-0.26.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.27.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts/data/scheme/variant.txt` & `sts_lib-0.27.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.26.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.27.0/sts_lib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.26.0
+Version: 0.27.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -35,38 +35,46 @@
 
 # STS 簡繁祕書
 
 STS (Simplified-Traditional Secretary) is an open library for flexible simplified-traditional Chinese text conversion.
 
 簡繁祕書是開源、輕巧、有彈性的中文簡繁轉換工具，也支援異體字轉換及地區慣用詞轉換。
 
+
 ## Features 特色
 
-* 使用與 [OpenCC](https://github.com/BYVoid/OpenCC) 格式相容的詞典檔。
+* 使用與 [OpenCC](https://github.com/BYVoid/OpenCC) 格式相容的詞典檔。此外亦支援 JSON 或 YAML 格式的詞典檔。
 * 可「並聯」或「串聯」組合多個詞典檔作為轉換方案，並預先儲存成單一詞典檔以加速載入。詞典檔更新時也會自動重新生成組合詞典。
 * 簡繁對應、異體字對應、地區慣用詞對應等不同的對應關係皆區分至不同的詞典檔。
 * 詞典及配置檔與程式本體分離，可自由修改、擴充。
 * 支援一對多轉換，轉換結果可輸出為純文字、HTML、JSON 等格式。
 * 支援 Unicode 組合字，例如「⿰虫鬼」視為一個字，不會因為詞典有「虫=>蟲」而被轉為「⿰蟲鬼」。
 * 支援用正規表示式略過特定文字的轉換。
 * 支援編碼轉換，可自訂輸入及輸出檔案的字元編碼。
 
+
 ## Usage 使用
 
 ### Installation 安裝
 
+安裝 Python >= 3.7 ([官網](https://www.python.org/))，然後在命令列輸入以下指令安裝（或升級至）最新版本：
+
     pip install -U sts-lib
 
+> 若要支援 YAML 格式，須額外安裝 PyYAML 套件，或改用以下指令安裝：
+>
+>    pip install -U sts-lib[yaml]
+
 ### Command Line
 
 * `sts --help` 或 `sts COMMAND --help` 檢視可用指令的詳細說明文檔。
 
 * `sts convert [OPTIONs] [file ...]` 執行簡繁轉換：
   * `file` 為一或多個欲轉換的檔案。（省略則讀取標準輸入 STDIN）
-  * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
+  * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製配置檔（JSON 或 YAML）的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如可輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
   * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return`（或 `return1`, `return2`, ... 等）子群組時會取代為子群組的值。
@@ -96,54 +104,129 @@
                        input_encoding='UTF-8', output_encoding='UTF-8',
                        format='txt', exclude=None)
 
 # perform a conversion for a string and process the result data generator
 [p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
 ```
 
-## Config 配置檔
+
+## Advanced 進階開發
+
+### Config 配置檔
+
+配置檔為 JSON 或 YAML 檔案（副檔名須為 `.yaml` 或 `.yml`）。規格如下：
 
 ```javascript
 /**
  * @typedef {Object} configScheme
  * @property {string} [name] - name/description of the config
  * @property {string[]} [requires] - required configs, which are made before
  *     making from this config, as an absolute path, or a path relative to the
  *     directory of this config file, or the basename of a built-in config file
- *     (with or without ".json")
- * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
+ *     (with or without extension ".json", ".yaml", ".yml")
+ * @property {srcDictScheme[]} dicts - schemes of each dictionary file to be
+ *     generated or loaded.
+ */
+
+/**
+ * A dictScheme or string for a dict.
+ *
+ * The string should be an absolute path, or a path relative to the directory
+ * of the config file, or the basename of a built-in dictionary file, with a
+ * file extension of .txt, .list, .json, .jlist, .yaml, or .yml.
+ *
+ * @typedef {(string|dictScheme)} srcDictScheme
  */
 
 /**
  * @typedef {Object} dictScheme
- * @property {string} file - path of the dictionary file to generate, as an
+ * @property {string} [file] - path of the dictionary file to generate, as an
  *     absolute path, or a path relative to the directory of this config file.
  *     It should be a .tlist (compiled trie), .jlist (compiled table), or .list
- *     (plain text table).
- * @property {string} [mode=load] - the mode to handle the loaded source files:
- *     "load" to simply merge the loaded keys and values; "swap" to reverse the
- *     dictionary (i.e. use the values as keys and the keys as values); "join"
- *     to build from a chain of dictionaries (in which case src must be an
- *     array of subarrays of strings)
- * @property {Array.<(string|string[])>} [src] - the source files. Each as an
- *     absolute path, or a path relative to the directory of this config file,
- *     or the basename of a built-in dictionary file. Each should be a .txt,
- *     .list, .json, .jlist, .yaml, or .yml dictionary file. File must exist
- *     when this is omitted.
+ *     (plain text table). An unknown file extension is treated as .list. `src`
+ *     must exist when omitted.
+ * @property {string} [mode=load] - the mode to handle the loaded dicts.
+ *     - "load" to simply merge the loaded keys and values;
+ *     - "swap" to reverse the dict (i.e. use the values as keys and the keys
+ *       as values);
+ *     - "join" to chain dicts (a conversion using a dict joining dict1 and
+ *       dict2 works like a conversion using dict1 and then dict2, but takes
+ *       care of word segmentation);
+ *     - "filter" to filter the output values in the loaded dicts with extra
+ *       "include" and "exclude" properties
+ *     - "expand" to expand the placeholders (defined in the extra
+ *       "placeholders" property) in the first dict with the matching key and
+ *        value in other dicts;
+ *     - "remove_keys" to remove keys from the first dict if it appears in any
+ *       other one;
+ *     - "remove_values" to remove key-value pairs from the first dict if it
+ *       appears in any other one.
+ * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
+ *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
- * @property {string} [include] - a regex filter that discards non-matched
- *     conversion values.
- * @property {string} [exclude] - a regex filter that discards matched
- *     conversion values.
  * @property {boolean} [check] - true to raise an exception if the output
  *     contains an invalid char which will be loaded incorrectly. Set this
  *     when the output is a plain text table file and the source files contain
  *     untrusted JSON or YAML data that may include a char like " ", "\t",
  *     "\n", etc. in the dictionary.
+ * @property {string} [include] - a regex filter that discards non-matched
+ *     conversion values. (for "filter" mode)
+ * @property {string} [exclude] - a regex filter that discards matched
+ *     conversion values. (for "filter" mode)
+ * @property {string[]} [placeholders] - strings to be expanded using other
+ *     dicts. (for "expand" mode)
  */
 ```
 
+### Dictionary 詞典檔
+
+原始詞典檔可為純文字、JSON、或 YAML。規格如下：
+
+#### 純文字
+
+純文字詞典副檔名為 .txt。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
+
+```
+輸入詞1\t轉換詞11 轉換詞12 ...
+輸入詞2\t轉換詞21 轉換詞22 ...
+...
+```
+
+注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外也不可含有換行等字元。
+
+#### JSON
+
+JSON 詞典副檔名為 `.json`。規格如下：
+
+```
+{
+  "輸入詞1": ["轉換詞11", "轉換詞12", ...],
+  "輸入詞2": ["轉換詞22", "轉換詞22", ...],
+  ...
+}
+```
+
+#### YAML
+
+YAML 詞典副檔名為 `.yaml` 或 `.yml`。規格如下：
+
+```
+輸入詞1: [轉換詞11, 轉換詞12, ...]
+輸入詞2: [轉換詞22, 轉換詞22, ...]
+...
+```
+
+
+## 線上版
+
+[簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
+
+本線上轉換工具支援文字轉換及檔案轉換。前者只要在輸入區填入文字，就會自動轉換並且可以互動式校訂。後者可以用按鈕或拖放選擇一或多個檔案，就會逐一轉換後自動下載。預設檔案輸入輸出編碼皆是UTF-8，如要輸入其他編碼的檔案，可在進階選項設定。
+
+目前內建 [OpenCC](https://github.com/BYVoid/OpenCC)、[MediaWiki](https://github.com/wikimedia/mediawiki)、[新同文堂](https://github.com/tongwentang/tongwen-dict)的轉換方案，並且修正了 OpenCC 演算法缺陷導致一些地區詞無法正常轉換的問題（詳見[相關問題回報](https://github.com/BYVoid/OpenCC/issues/475)）。
+
+
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
 
 詞典檔原始資料來自同文堂、維基百科、OpenCC 等開源專案，再按本專案之需求編校。
```

### Comparing `sts_lib-0.26.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.27.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

