# Comparing `tmp/ALLM-1.0-py3-none-any.whl.zip` & `tmp/ALLM-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6701 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLM/__init__.py
--rw-rw-rw-  2.0 fat     1904 b- defN 24-Apr-20 05:31 ALLM/api.py
--rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLM/cli.py
--rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLM/generate.py
--rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLM/instruct.py
--rw-rw-rw-  2.0 fat     2371 b- defN 24-Apr-20 10:51 ALLM-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 10:51 ALLM-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       81 b- defN 24-Apr-20 10:51 ALLM-1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-20 10:51 ALLM-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      720 b- defN 24-Apr-20 10:51 ALLM-1.0.dist-info/RECORD
-10 files, 18882 bytes uncompressed, 5493 bytes compressed:  70.9%
+Zip file size: 6726 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-21 10:37 ALLM/__init__.py
+-rw-rw-rw-  2.0 fat     1911 b- defN 24-Apr-21 16:12 ALLM/api.py
+-rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-21 10:37 ALLM/cli.py
+-rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-21 10:37 ALLM/generate.py
+-rw-rw-rw-  2.0 fat    10338 b- defN 24-Apr-21 17:50 ALLM/instruct.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       75 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      730 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/RECORD
+10 files, 18898 bytes uncompressed, 5498 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: ALLM/generate.py
 Comment: 
 
 Filename: ALLM/instruct.py
 Comment: 
 
-Filename: ALLM-1.0.dist-info/METADATA
+Filename: ALLM-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: ALLM-1.0.dist-info/WHEEL
+Filename: ALLM-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: ALLM-1.0.dist-info/entry_points.txt
+Filename: ALLM-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLM-1.0.dist-info/top_level.txt
+Filename: ALLM-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLM-1.0.dist-info/RECORD
+Filename: ALLM-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLM/api.py

```diff
@@ -29,15 +29,15 @@
         return "Exiting chat."
     response_iter = llm.stream_complete(prompt)
     response_text = ''.join(response.delta for response in response_iter)
     return response_text
 
 @app.route('/')
 def index():
-    return "Welcome to the allmdev API!"
+    return "Welcome to the All Advance AI API!"
 
 @app.route('/v1/chat/completions', methods=['POST'])
 def infer_text():
     user_input = request.data.decode('utf-8')
     print("Received input:", user_input)  # Debug statement
 
     if model_path is None:
```

## ALLM/instruct.py

```diff
@@ -148,15 +148,15 @@
             verbose=False,
         )
 
         # Start the chat loop
         while True:
             try:
                 # Prompt user for input
-                user_input = input("User: ")
+                user_input = input("\n\nUser: ")
                 
                 # Exit loop if user types "exit"
                 if user_input.lower() == "exit":
                     print("Exiting chat.")
                     break
                 
                 # Construct prompt with user input
```

## Comparing `ALLM-1.0.dist-info/METADATA` & `ALLM-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ALLM
-Version: 1.0
+Version: 1.0.1
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Abdul Mannan Khan
-Maintainer-email: abbdulmannan.khan@allaai.com
+Maintainer-email: abdulmannan.khan@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
 Requires-Dist: Flask
 Requires-Dist: click
 Requires-Dist: llama-index
 Requires-Dist: llama-cpp-python
 Requires-Dist: aiohttp
```

## Comparing `ALLM-1.0.dist-info/RECORD` & `ALLM-1.0.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ALLM/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
-ALLM/api.py,sha256=Y69wMrLgODKsoiWQRH9CCVLU4IA8QYO9rX3C0fciEGI,1904
+ALLM/api.py,sha256=wkihJbxEWe69LL66RuiDJqZYWiLR2nnQ7rb1AVMhFiQ,1911
 ALLM/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
 ALLM/generate.py,sha256=bjvXRrlHpe_-TsWDAL-OoivuTO9225gOK15FKRlBvIg,2579
-ALLM/instruct.py,sha256=9cjx7CnIc-C-LXxVl2THdlrNX3WXcZ0rXKXWVpZ0BXY,10334
-ALLM-1.0.dist-info/METADATA,sha256=2l61YOCLNfHlhawKe6_WVBiKmfhE8SnPw2VduwOdWPQ,2371
-ALLM-1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLM-1.0.dist-info/entry_points.txt,sha256=Vg1PNkMT6_InD8pcRNpouHe5eJ-VSb9lWSb7XeeJr1o,81
-ALLM-1.0.dist-info/top_level.txt,sha256=7I9ZpiXpdc4mz6ZgmIvmsbw5M2OC1m99v28mTvj1qEM,5
-ALLM-1.0.dist-info/RECORD,,
+ALLM/instruct.py,sha256=2tasQjI3gQOmTudcVCg04Y1Wu9EICZTHNCDxEmF61GA,10338
+ALLM-1.0.1.dist-info/METADATA,sha256=oZBwc6HK5DHN6OBSn-2geOb33X3JZcyxO76SKc7iJJw,2372
+ALLM-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLM-1.0.1.dist-info/entry_points.txt,sha256=bRVlAhmjDquIZd9PRF-QVLXaA7gGWr9F9TOMkX4lGgA,75
+ALLM-1.0.1.dist-info/top_level.txt,sha256=7I9ZpiXpdc4mz6ZgmIvmsbw5M2OC1m99v28mTvj1qEM,5
+ALLM-1.0.1.dist-info/RECORD,,
```

