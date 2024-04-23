# Comparing `tmp/scrapy_contrib-0.0.6-py3-none-any.whl.zip` & `tmp/scrapy_contrib-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 157451 bytes, number of entries: 9
+Zip file size: 135829 bytes, number of entries: 8
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 scrapylib/plugins/__init__.py
--rw-r--r--  2.0 fat   161792 b- defN 20-Feb-02 00:00 scrapylib/plugins/core.cp310-win_amd64.pyd
--rw-r--r--  2.0 fat    84480 b- defN 20-Feb-02 00:00 scrapylib/plugins/coreType.cp310-win_amd64.pyd
--rw-r--r--  2.0 fat    47104 b- defN 20-Feb-02 00:00 scrapylib/plugins/ltype.cp310-win_amd64.pyd
--rw-r--r--  2.0 fat    74752 b- defN 20-Feb-02 00:00 scrapylib/plugins/parse.cp310-win_amd64.pyd
-?rw-r--r--  2.0 fat     1689 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.6.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1093 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.6.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      821 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.6.dist-info/RECORD
-9 files, 371818 bytes uncompressed, 156021 bytes compressed:  58.0%
+-rw-r--r--  2.0 fat   123904 b- defN 20-Feb-02 00:00 scrapylib/plugins/scrapy_lib.cp310-win_amd64.pyd
+-rw-r--r--  2.0 fat   121856 b- defN 20-Feb-02 00:00 scrapylib/plugins/scrapy_parse.cp310-win_amd64.pyd
+-rw-r--r--  2.0 fat    50688 b- defN 20-Feb-02 00:00 scrapylib/plugins/scrapy_reader.cp310-win_amd64.pyd
+?rw-r--r--  2.0 fat     1689 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.8.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1093 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      739 b- defN 20-Feb-02 00:00 scrapy_contrib-0.0.8.dist-info/RECORD
+8 files, 300056 bytes uncompressed, 134525 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
 Filename: scrapylib/plugins/__init__.py
 Comment: 
 
-Filename: scrapylib/plugins/core.cp310-win_amd64.pyd
+Filename: scrapylib/plugins/scrapy_lib.cp310-win_amd64.pyd
 Comment: 
 
-Filename: scrapylib/plugins/coreType.cp310-win_amd64.pyd
+Filename: scrapylib/plugins/scrapy_parse.cp310-win_amd64.pyd
 Comment: 
 
-Filename: scrapylib/plugins/ltype.cp310-win_amd64.pyd
+Filename: scrapylib/plugins/scrapy_reader.cp310-win_amd64.pyd
 Comment: 
 
-Filename: scrapylib/plugins/parse.cp310-win_amd64.pyd
+Filename: scrapy_contrib-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: scrapy_contrib-0.0.6.dist-info/METADATA
+Filename: scrapy_contrib-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: scrapy_contrib-0.0.6.dist-info/WHEEL
+Filename: scrapy_contrib-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: scrapy_contrib-0.0.6.dist-info/licenses/LICENSE
-Comment: 
-
-Filename: scrapy_contrib-0.0.6.dist-info/RECORD
+Filename: scrapy_contrib-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `scrapy_contrib-0.0.6.dist-info/METADATA` & `scrapy_contrib-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scrapy_contrib
-Version: 0.0.6
+Version: 0.0.8
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
```

## Comparing `scrapy_contrib-0.0.6.dist-info/licenses/LICENSE` & `scrapy_contrib-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

