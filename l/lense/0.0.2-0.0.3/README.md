# Comparing `tmp/lense-0.0.2-py3-none-any.whl.zip` & `tmp/lense-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,6 @@
-Zip file size: 7865 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       24 b- defN 24-Apr-11 09:48 lense/__init__.py
--rw-rw-rw-  2.0 fat      455 b- defN 24-Apr-15 12:02 lense/app.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 06:48 lense/_chat/__init__.py
--rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-15 11:44 lense/_chat/cglense.py
--rw-rw-rw-  2.0 fat     6653 b- defN 24-Apr-15 11:55 lense/_chat/engine.py
--rw-rw-rw-  2.0 fat     4850 b- defN 24-Apr-15 11:45 lense/_chat/error_handling.py
--rw-rw-rw-  2.0 fat     4179 b- defN 24-Apr-15 11:48 lense/_chat/loader.py
--rw-rw-rw-  2.0 fat      519 b- defN 24-Apr-15 11:45 lense/_chat/replace_file.py
--rw-rw-rw-  2.0 fat      653 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      909 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/RECORD
-12 files, 19513 bytes uncompressed, 6347 bytes compressed:  67.5%
+Zip file size: 1187 bytes, number of entries: 4
+-rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-22 09:16 lense-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 09:16 lense-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-22 09:16 lense-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      288 b- defN 24-Apr-22 09:16 lense-0.0.3.dist-info/RECORD
+4 files, 1311 bytes uncompressed, 621 bytes compressed:  52.6%
```

## zipnote {}

```diff
@@ -1,37 +1,13 @@
-Filename: lense/__init__.py
+Filename: lense-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: lense/app.py
+Filename: lense-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: lense/_chat/__init__.py
+Filename: lense-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lense/_chat/cglense.py
-Comment: 
-
-Filename: lense/_chat/engine.py
-Comment: 
-
-Filename: lense/_chat/error_handling.py
-Comment: 
-
-Filename: lense/_chat/loader.py
-Comment: 
-
-Filename: lense/_chat/replace_file.py
-Comment: 
-
-Filename: lense-0.0.2.dist-info/METADATA
-Comment: 
-
-Filename: lense-0.0.2.dist-info/WHEEL
-Comment: 
-
-Filename: lense-0.0.2.dist-info/top_level.txt
-Comment: 
-
-Filename: lense-0.0.2.dist-info/RECORD
+Filename: lense-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lense-0.0.2.dist-info/METADATA` & `lense-0.0.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: lense
-Version: 0.0.2
+Version: 0.0.3
 Requires-Dist: pandas ==2.2.2
 Requires-Dist: PyPDF2 ==3.0.1
 Requires-Dist: python-docx ==1.1.0
 Requires-Dist: python-pptx ==0.6.23
 Requires-Dist: llama-index ==0.10.29
 Requires-Dist: llama-index.llms.azure-openai ==0.1.5
 Requires-Dist: llama-index.embeddings.azure-openai ==0.1.6
 Requires-Dist: langchain ==0.1.16
 Requires-Dist: huggingface-hub ==0.22.2
 Requires-Dist: PyMuPDF ==1.24.1
 Requires-Dist: sentence-transformers ==2.6.1
 Requires-Dist: llama-index-embeddings-langchain ==0.1.2
 Requires-Dist: llama-index-llms-langchain ==0.1.3
 Requires-Dist: llama-index.experimental ==0.1.3
+Requires-Dist: langchain-google-genai ==1.0.2
+Requires-Dist: langchain-experimental ==0.0.57
+Requires-Dist: langchain-openai ==0.1.3
+Requires-Dist: psycopg2 ==2.9.9
+Requires-Dist: fastapi ==0.110.2
+Requires-Dist: python-multipart ==0.0.9
+Requires-Dist: uvicorn ==0.29.0
```

