# Comparing `tmp/sts_lib-0.27.0.tar.gz` & `tmp/sts_lib-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.27.0.tar", last modified: Tue Apr 23 04:16:18 2024, max compression
+gzip compressed data, was "sts_lib-0.27.1.tar", last modified: Tue Apr 23 08:28:03 2024, max compression
```

## Comparing `sts_lib-0.27.0.tar` & `sts_lib-0.27.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.045346 sts_lib-0.27.0/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10790 2024-04-23 04:16:18.044347 sts_lib-0.27.0/PKG-INFO
--rw-rw-rw-   0        0        0     9337 2024-04-23 04:11:40.000000 sts_lib-0.27.0/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-23 04:16:18.046345 sts_lib-0.27.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:17.999124 sts_lib-0.27.0/sts/
--rw-rw-rw-   0        0        0    52284 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-23 03:16:40.000000 sts_lib-0.27.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.000104 sts_lib-0.27.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.014962 sts_lib-0.27.0/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.031403 sts_lib-0.27.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-23 04:12:14.000000 sts_lib-0.27.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22760 2024-04-23 02:29:50.000000 sts_lib-0.27.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.035384 sts_lib-0.27.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-23 04:11:40.000000 sts_lib-0.27.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 04:16:18.042349 sts_lib-0.27.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0    10790 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-23 04:16:17.000000 sts_lib-0.27.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.696675 sts_lib-0.27.1/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.1/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11018 2024-04-23 08:28:03.696675 sts_lib-0.27.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9565 2024-04-23 08:25:00.000000 sts_lib-0.27.1/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-23 08:28:03.697674 sts_lib-0.27.1/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.652673 sts_lib-0.27.1/sts/
+-rw-rw-rw-   0        0        0    52645 2024-04-23 08:25:00.000000 sts_lib-0.27.1/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.1/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-23 08:11:31.000000 sts_lib-0.27.1/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.653672 sts_lib-0.27.1/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.670701 sts_lib-0.27.1/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.684514 sts_lib-0.27.1/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22760 2024-04-23 08:00:20.000000 sts_lib-0.27.1/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.687516 sts_lib-0.27.1/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.693678 sts_lib-0.27.1/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0    11018 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.27.0/LICENSE` & `sts_lib-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/PKG-INFO` & `sts_lib-0.27.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.0
+Version: 0.27.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -151,15 +151,15 @@
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
  *     - "filter" to filter the output values in the loaded dicts with extra
  *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
- *        value in other dicts;
+ *        values in other dicts;
  *     - "remove_keys" to remove keys from the first dict if it appears in any
  *       other one;
  *     - "remove_values" to remove key-value pairs from the first dict if it
  *       appears in any other one.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
@@ -175,47 +175,49 @@
  * @property {string[]} [placeholders] - strings to be expanded using other
  *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
-原始詞典檔可為純文字、JSON、或 YAML。規格如下：
+原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
 
 #### 純文字
 
-純文字詞典副檔名為 .txt。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
+純文字詞典副檔名為 `.txt` 或 `.list`。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
 
 ```
 輸入詞1\t轉換詞11 轉換詞12 ...
 輸入詞2\t轉換詞21 轉換詞22 ...
 ...
 ```
 
-注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外也不可含有換行等字元。
+注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外二者也不可含有換行等字元。
 
 #### JSON
 
-JSON 詞典副檔名為 `.json`。規格如下：
+JSON 詞典副檔名為 `.json` 或 `.jlist`。規格如下：
 
 ```
 {
-  "輸入詞1": ["轉換詞11", "轉換詞12", ...],
-  "輸入詞2": ["轉換詞22", "轉換詞22", ...],
+  "輸入詞1": "轉換詞11",
+  "輸入詞2": ["轉換詞21"],
+  "輸入詞3": ["轉換詞31", "轉換詞32", ...],
   ...
 }
 ```
 
 #### YAML
 
 YAML 詞典副檔名為 `.yaml` 或 `.yml`。規格如下：
 
 ```
-輸入詞1: [轉換詞11, 轉換詞12, ...]
-輸入詞2: [轉換詞22, 轉換詞22, ...]
+輸入詞1: 轉換詞11
+輸入詞2: [轉換詞21]
+輸入詞3: [轉換詞31, 轉換詞32, ...]
 ...
 ```
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
```

### Comparing `sts_lib-0.27.0/README.md` & `sts_lib-0.27.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,15 @@
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
  *     - "filter" to filter the output values in the loaded dicts with extra
  *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
- *        value in other dicts;
+ *        values in other dicts;
  *     - "remove_keys" to remove keys from the first dict if it appears in any
  *       other one;
  *     - "remove_values" to remove key-value pairs from the first dict if it
  *       appears in any other one.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
@@ -140,47 +140,49 @@
  * @property {string[]} [placeholders] - strings to be expanded using other
  *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
-原始詞典檔可為純文字、JSON、或 YAML。規格如下：
+原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
 
 #### 純文字
 
-純文字詞典副檔名為 .txt。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
+純文字詞典副檔名為 `.txt` 或 `.list`。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
 
 ```
 輸入詞1\t轉換詞11 轉換詞12 ...
 輸入詞2\t轉換詞21 轉換詞22 ...
 ...
 ```
 
-注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外也不可含有換行等字元。
+注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外二者也不可含有換行等字元。
 
 #### JSON
 
-JSON 詞典副檔名為 `.json`。規格如下：
+JSON 詞典副檔名為 `.json` 或 `.jlist`。規格如下：
 
 ```
 {
-  "輸入詞1": ["轉換詞11", "轉換詞12", ...],
-  "輸入詞2": ["轉換詞22", "轉換詞22", ...],
+  "輸入詞1": "轉換詞11",
+  "輸入詞2": ["轉換詞21"],
+  "輸入詞3": ["轉換詞31", "轉換詞32", ...],
   ...
 }
 ```
 
 #### YAML
 
 YAML 詞典副檔名為 `.yaml` 或 `.yml`。規格如下：
 
 ```
-輸入詞1: [轉換詞11, 轉換詞12, ...]
-輸入詞2: [轉換詞22, 轉換詞22, ...]
+輸入詞1: 轉換詞11
+輸入詞2: [轉換詞21]
+輸入詞3: [轉換詞31, 轉換詞32, ...]
 ...
 ```
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
```

### Comparing `sts_lib-0.27.0/setup.cfg` & `sts_lib-0.27.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/__init__.py` & `sts_lib-0.27.1/sts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.27.0'
+__version__ = '0.27.1'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -202,16 +202,15 @@
           key2 <tab> value2-1 [<space> value2-2 <space> ...]
           ...
 
     - JSON: which is dumped from the internal data structure.
     """
     def __init__(self, *args, **kwargs):
         self._dict = {}
-        for key, values in dict(*args, **kwargs).items():
-            self.add(key, values, skip_check=True)
+        self.update(dict(*args, **kwargs))
 
     def __repr__(self):
         """Implementation of repr(self).
         """
         return f'{self.__class__.__name__}({repr(list(self.items()))})'
 
     def __getitem__(self, key):
@@ -276,20 +275,20 @@
         """
         yield from self._dict.items()
 
     def add(self, key, values, skip_check=False):
         """Add a key-values pair to this dictionary.
 
         Args:
-            values: a string or a list of strings.
+            values: a string or an iterable of strings.
             skip_check: True to skip checking duplicated values.
         """
-        values = [values] if isinstance(values, str) else values
+        values = (values,) if isinstance(values, str) else values
         list_ = self._dict.setdefault(key, [])
-        list_ += values if skip_check else [x for x in values if x not in list_]
+        list_ += values if skip_check else (x for x in values if x not in list_)
         return self
 
     def update(self, stsdict, skip_check=False):
         """Add all key-values pairs from another StsDict or dict.
 
         Args:
             skip_check: True to skip checking duplicated values.
@@ -320,29 +319,27 @@
                     self.add(key, values.split(' '))
 
     def _load_json(self, file):
         with open(file, 'r', encoding='UTF-8') as fh:
             data = json.load(fh)
             if not isinstance(data, dict):
                 data = dict(data)
-            for key, values in data.items():
-                self.add(key, values)
+            self.update(data)
 
     def _load_yaml(self, file):
         try:
             import yaml
         except ModuleNotFoundError:
             raise RuntimeError('install PyYAML module to support loading .yaml files')
 
         with open(file, 'r', encoding='UTF-8') as fh:
             data = yaml.safe_load(fh)
             if not isinstance(data, dict):
                 data = dict(data)
-            for key, values in data.items():
-                self.add(key, values)
+            self.update(data)
 
     def dump(self, file=None, sort=False, check=False):
         """Dump key-values pairs to a plain-dict file.
 
         Args:
             file: path of file to save. Use stdout if None.
             sort: True to sort the output.
@@ -1074,15 +1071,15 @@
                 dict_scheme['exclude'] = None
             except re.error as exc:
                 raise ValueError(f'regex syntax error of the "exclude" filter: {exc}')
 
         elif mode == 'expand':
             dict_scheme.setdefault('placeholders', [])
             if len(dict_scheme['placeholders']) != len(srcs) - 1:
-                raise ValueError('length of dict["placeholders"] does not match dict["src"]')
+                raise ValueError('len(dict["placeholders"]) must be len(dict["src"]) - 1')
 
         return dict_scheme
 
     def make_dict(self, dict_scheme, config_dir, skip_check=False, quiet=False):
         """Make a dict.
 
         Returns:
@@ -1135,16 +1132,15 @@
 
     def _make_dict_mode_load(self, dict_scheme):
         table = Table()
         for src in dict_scheme['src']:
             if isinstance(src, str):
                 table.load(src)
             else:
-                for key, values in src.items():
-                    table.add(key, values)
+                table.update(src)
         return table
 
     def _make_dict_mode_filter(self, dict_scheme):
         table = self._make_dict_mode_load(dict_scheme)
 
         include = dict_scheme['include']
         exclude = dict_scheme['exclude']
@@ -1178,35 +1174,40 @@
         srcs = dict_scheme['src']
         src = srcs.pop(0)
         table = Table().load(src) if isinstance(src, str) else src
         dicts = [Table().load(src) if isinstance(src, str) else src for src in srcs]
 
         placeholders = dict_scheme['placeholders']
         placeholders_re = re.compile('|'.join(re.escape(p) for p in placeholders))
-        map_placeholder_to_idx = {p: i for i, p in enumerate(placeholders)}
+        map_ph_to_dict_idx = {p: i for i, p in enumerate(placeholders)}
 
         for key, values in table.items():
             key_parts = list(self._make_dict_mode_expand_split(key, placeholders_re))
             value_parts_list = [list(self._make_dict_mode_expand_split(v, placeholders_re)) for v in values]
 
-            map_placeholder_to_dict_keys = {}
+            map_ph_to_comb_idx = {}
             for part in itertools.chain(key_parts, *value_parts_list):
                 if isinstance(part, str):
                     continue
-                key = part[0]
-                key_idx = map_placeholder_to_idx[key]
-                dict_keys = dicts[key_idx].keys()
-                map_placeholder_to_dict_keys[key] = dict_keys
-
-            for comb in itertools.product(*map_placeholder_to_dict_keys.values()):
-                newkey = self._make_dict_mode_expand_get_expanded_key(key_parts, comb, map_placeholder_to_idx)
-                newvalues = [
-                    self._make_dict_mode_expand_get_expanded_value(vpp, comb, map_placeholder_to_idx, dicts)
+                ph = part[0]
+                map_ph_to_comb_idx.setdefault(ph, len(map_ph_to_comb_idx))
+
+            # shortcut when no placeholder
+            if not map_ph_to_comb_idx:
+                newtable.add(key, values)
+                continue
+
+            it = (dicts[map_ph_to_dict_idx[ph]] for ph in map_ph_to_comb_idx)
+            for comb in itertools.product(*it):
+                context = (dicts, comb, map_ph_to_dict_idx, map_ph_to_comb_idx)
+                newkey = self._make_dict_mode_expand_get_expanded_key(key_parts, context)
+                newvalues = itertools.chain.from_iterable(
+                    self._make_dict_mode_expand_get_expanded_values(vpp, context)
                     for vpp in value_parts_list
-                ]
+                )
                 newtable.add(newkey, newvalues)
 
         return newtable
 
     @staticmethod
     def _make_dict_mode_expand_split(text, placeholders_re):
         index = 0
@@ -1224,41 +1225,53 @@
             index = end
 
         t = text[index:]
         if t:
             yield t
 
     @staticmethod
-    def _make_dict_mode_expand_get_expanded_key(parts, comb, map_placeholder_to_idx):
+    def _make_dict_mode_expand_get_expanded_key(parts, context):
+        _, comb, _, map_ph_to_comb_idx = context
         rv = []
         for part in parts:
             if isinstance(part, str):
                 rv.append(part)
                 continue
 
-            key = part[0]
-            key_idx = map_placeholder_to_idx[key]
-            rv.append(comb[key_idx])
+            ph = part[0]
+            rv.append(comb[map_ph_to_comb_idx[ph]])
         return ''.join(rv)
 
     @staticmethod
-    def _make_dict_mode_expand_get_expanded_value(parts, comb, map_placeholder_to_idx, dicts):
+    def _make_dict_mode_expand_get_expanded_values(parts, context):
+        dicts, comb, map_ph_to_dict_idx, map_ph_to_comb_idx = context
         rv = []
-        for part in parts:
+        stack = [(parts, 0)]
+        substack = []
+        while stack:
+            parts, idx = stack.pop()
+            try:
+                part = parts[idx]
+            except IndexError:
+                rv.append(''.join(parts))
+                continue
+
             if isinstance(part, str):
-                rv.append(part)
+                stack.append((parts, idx + 1))
                 continue
 
-            key = part[0]
-            key_idx = map_placeholder_to_idx[key]
-            try:
-                rv.append(dicts[key_idx][comb[key_idx]][0])
-            except IndexError:
-                rv.append(key)
-        return ''.join(rv)
+            ph = part[0]
+            dict_idx = map_ph_to_dict_idx[ph]
+            comb_idx = map_ph_to_comb_idx[ph]
+            for value in dicts[dict_idx][comb[comb_idx]]:
+                newparts = parts[:idx] + [value] + parts[idx + 1:]
+                substack.append((newparts, idx + 1))
+            while substack:
+                stack.append(substack.pop())
+        return rv
 
     def _make_dict_mode_remove_keys(self, dict_scheme):
         srcs = dict_scheme['src']
         src = srcs.pop(0)
         table = Table().load(src) if isinstance(src, str) else src
         for src in srcs:
             dict_ = Table().load(src) if isinstance(src, str) else src
```

### Comparing `sts_lib-0.27.0/sts/cli.py` & `sts_lib-0.27.1/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/config/_default.json` & `sts_lib-0.27.1/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/config/hk2s.json` & `sts_lib-0.27.1/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/config/s2twp.json` & `sts_lib-0.27.1/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/config/tw2s.json` & `sts_lib-0.27.1/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/config/tw2sp.json` & `sts_lib-0.27.1/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.27.1/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.27.1/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.27.1/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.27.1/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.27.1/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.27.1/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.27.1/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.27.1/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.27.1/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.27.1/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts/data/scheme/variant.txt` & `sts_lib-0.27.1/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.27.1/sts_lib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.0
+Version: 0.27.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -151,15 +151,15 @@
  *     - "join" to chain dicts (a conversion using a dict joining dict1 and
  *       dict2 works like a conversion using dict1 and then dict2, but takes
  *       care of word segmentation);
  *     - "filter" to filter the output values in the loaded dicts with extra
  *       "include" and "exclude" properties
  *     - "expand" to expand the placeholders (defined in the extra
  *       "placeholders" property) in the first dict with the matching key and
- *        value in other dicts;
+ *        values in other dicts;
  *     - "remove_keys" to remove keys from the first dict if it appears in any
  *       other one;
  *     - "remove_values" to remove key-value pairs from the first dict if it
  *       appears in any other one.
  * @property {srcDictScheme[]} [src] - the source dicts. `file` must exist when
  *     omitted.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
@@ -175,47 +175,49 @@
  * @property {string[]} [placeholders] - strings to be expanded using other
  *     dicts. (for "expand" mode)
  */
 ```
 
 ### Dictionary 詞典檔
 
-原始詞典檔可為純文字、JSON、或 YAML。規格如下：
+原始詞典檔可為純文字、JSON、或 YAML。編譯產生的詞典檔有純文字（`.list`）、JSON列表（`.jlist`）、JSON樹（`.tlist`）三種格式，其中前二者可再作為原始檔輸入，後者則只能用於轉換。
 
 #### 純文字
 
-純文字詞典副檔名為 .txt。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
+純文字詞典副檔名為 `.txt` 或 `.list`。規格為以 TAB 字元分隔輸入詞與轉換詞，多個轉換詞之間以半形空白分隔，如下：
 
 ```
 輸入詞1\t轉換詞11 轉換詞12 ...
 輸入詞2\t轉換詞21 轉換詞22 ...
 ...
 ```
 
-注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外也不可含有換行等字元。
+注意，使用此格式時，輸入詞不可含有 TAB 字元，轉換詞不可含有半形空白字元。此外二者也不可含有換行等字元。
 
 #### JSON
 
-JSON 詞典副檔名為 `.json`。規格如下：
+JSON 詞典副檔名為 `.json` 或 `.jlist`。規格如下：
 
 ```
 {
-  "輸入詞1": ["轉換詞11", "轉換詞12", ...],
-  "輸入詞2": ["轉換詞22", "轉換詞22", ...],
+  "輸入詞1": "轉換詞11",
+  "輸入詞2": ["轉換詞21"],
+  "輸入詞3": ["轉換詞31", "轉換詞32", ...],
   ...
 }
 ```
 
 #### YAML
 
 YAML 詞典副檔名為 `.yaml` 或 `.yml`。規格如下：
 
 ```
-輸入詞1: [轉換詞11, 轉換詞12, ...]
-輸入詞2: [轉換詞22, 轉換詞22, ...]
+輸入詞1: 轉換詞11
+輸入詞2: [轉換詞21]
+輸入詞3: [轉換詞31, 轉換詞32, ...]
 ...
 ```
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
```

### Comparing `sts_lib-0.27.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.27.1/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

