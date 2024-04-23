# Comparing `tmp/lense-0.0.5-py3-none-any.whl.zip` & `tmp/lense-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9943 bytes, number of entries: 14
+Zip file size: 9978 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-22 06:00 lense/__init__.py
--rw-rw-rw-  2.0 fat     6527 b- defN 24-Apr-23 07:49 lense/app.py
--rw-rw-rw-  2.0 fat     3290 b- defN 24-Apr-22 07:32 lense/lense/SQL_engine.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-22 06:59 lense/lense/__init__.py
--rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-22 07:20 lense/lense/cglense.py
--rw-rw-rw-  2.0 fat     5836 b- defN 24-Apr-22 07:22 lense/lense/csv_engine.py
--rw-rw-rw-  2.0 fat     4694 b- defN 24-Apr-22 07:24 lense/lense/error_handling.py
--rw-rw-rw-  2.0 fat     1060 b- defN 24-Apr-23 07:49 lense/lense/loader.py
--rw-rw-rw-  2.0 fat     2464 b- defN 24-Apr-22 07:28 lense/lense/qna_engine.py
--rw-rw-rw-  2.0 fat     3336 b- defN 24-Apr-22 07:31 lense/lense/replace_file.py
--rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1079 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/RECORD
-14 files, 30509 bytes uncompressed, 8165 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat     6494 b- defN 24-Apr-23 07:59 lense/app.py
+-rw-rw-rw-  2.0 fat     3290 b- defN 24-Apr-22 07:32 lense/backend/SQL_engine.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-22 06:59 lense/backend/__init__.py
+-rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-22 07:20 lense/backend/cglense.py
+-rw-rw-rw-  2.0 fat     5836 b- defN 24-Apr-22 07:22 lense/backend/csv_engine.py
+-rw-rw-rw-  2.0 fat     4694 b- defN 24-Apr-22 07:24 lense/backend/error_handling.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 24-Apr-23 07:54 lense/backend/loader.py
+-rw-rw-rw-  2.0 fat     2464 b- defN 24-Apr-22 07:28 lense/backend/qna_engine.py
+-rw-rw-rw-  2.0 fat     3336 b- defN 24-Apr-22 07:31 lense/backend/replace_file.py
+-rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 08:00 lense-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 08:00 lense-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 08:00 lense-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1095 b- defN 24-Apr-23 08:00 lense-0.0.6.dist-info/RECORD
+14 files, 30496 bytes uncompressed, 8168 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
 Filename: lense/__init__.py
 Comment: 
 
 Filename: lense/app.py
 Comment: 
 
-Filename: lense/lense/SQL_engine.py
+Filename: lense/backend/SQL_engine.py
 Comment: 
 
-Filename: lense/lense/__init__.py
+Filename: lense/backend/__init__.py
 Comment: 
 
-Filename: lense/lense/cglense.py
+Filename: lense/backend/cglense.py
 Comment: 
 
-Filename: lense/lense/csv_engine.py
+Filename: lense/backend/csv_engine.py
 Comment: 
 
-Filename: lense/lense/error_handling.py
+Filename: lense/backend/error_handling.py
 Comment: 
 
-Filename: lense/lense/loader.py
+Filename: lense/backend/loader.py
 Comment: 
 
-Filename: lense/lense/qna_engine.py
+Filename: lense/backend/qna_engine.py
 Comment: 
 
-Filename: lense/lense/replace_file.py
+Filename: lense/backend/replace_file.py
 Comment: 
 
-Filename: lense-0.0.5.dist-info/METADATA
+Filename: lense-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: lense-0.0.5.dist-info/WHEEL
+Filename: lense-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: lense-0.0.5.dist-info/top_level.txt
+Filename: lense-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: lense-0.0.5.dist-info/RECORD
+Filename: lense-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lense/app.py

```diff
@@ -1,17 +1,17 @@
 #from loader import load_document
-from lense.lense.qna_engine import *
-from lense.lense.SQL_engine import *
-from lense.lense.csv_engine import *
+from lense.backend.qna_engine import *
+from lense.backend.SQL_engine import *
+from lense.backend.csv_engine import *
 from fastapi import FastAPI, File, UploadFile, Form
 from enum import Enum
-from lense.lense.qna_engine import embed_and_run_openai, embed_and_run_azureopenai, embed_and_run_mistral
+from lense.backend.qna_engine import embed_and_run_openai, embed_and_run_azureopenai, embed_and_run_mistral
 import shutil
 import os
-from lense.lense.loader import load_document
+from lense.backend.loader import load_document
 from fastapi import FastAPI, Request ,APIRouter
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 import uvicorn
 
 
 app = FastAPI()
@@ -29,15 +29,15 @@
 # List to store engines
 engines = []
 
 uploaded_file_path = None
 
 
 @app.post("/upload/")
-async def upload_file(file: UploadFile = File(...)):
+def upload_file(file: UploadFile = File(...)):
     global uploaded_file_path
     try:
         # Save the uploaded file to the temporary directory
         save_path = f"{file.filename}"
         with open(save_path, "wb") as buffer:
             shutil.copyfileobj(file.file, buffer)
         
@@ -48,15 +48,15 @@
     
     except Exception as e:
         return {"error": str(e)}
     
     
 
 @app.post("/process_document/")
-async def process_document(
+def process_document(
     engine_type: EngineType,
     api_key: str = Form(None),
     api_version: str = Form(None),
     azure_endpoint: str = Form(None),
     hf_token: str = Form(None)
 ):
     global uploaded_file_path
@@ -106,32 +106,32 @@
         
         return {"result": "Engine created and stored successfully"}
     
     except Exception as e:
         return {"error": str(e)}
     
 @app.post("/use-engine_document/")
-async def use_engine(
+def use_engine(
     query: str = Form(...)
-):
+     ):
     try:
         # Check if any engine has been stored
         if not engines:
             return {"error": "No engine available"}
         
         # Use the latest stored engine to run the query
         engine = engines[-1]
         result = engine(query)
 
         return {"result": str(result)}
     
     except Exception as e:
         return {"error": str(e)}
 @app.post("/process_csv/")
-async def process_document(
+def process_document(
     engine_type: EngineType1,
     api_key: str = Form(None),
     api_version: str = Form(None),
     azure_endpoint: str = Form(None)
 ):
     global uploaded_file_path
     try:
@@ -173,15 +173,15 @@
         
         return {"result": "Engine created and stored successfully"}
     
     except Exception as e:
         return {"error": str(e)}
     
 @app.post("/use-engine_csv/")
-async def use_engine(
+def use_engine(
     query: str = Form(...)
 ):
     try:
         # Check if any engine has been stored
         if not engines:
             return {"error": "No engine available"}
         
@@ -193,9 +193,9 @@
         return {"result": result}
     
     except Exception as e:
         return {"error": str(e)}
     
 
 def start():
-    app.mount("/", StaticFiles(directory="lense/lense/my_frontend", html=True), name="lense/lense/my_frontend")
-    uvicorn.run("lense.lense.app:app", reload=False, host="127.0.0.1", port=9009,workers=1)
+    app.mount("/", StaticFiles(directory="lense/my_frontend", html=True), name="lense/my_frontend")
+    uvicorn.run("lense.app:app", reload=False, host="127.0.0.1", port=9009,workers=1)
```

## Comparing `lense/lense/SQL_engine.py` & `lense/backend/SQL_engine.py`

 * *Files identical despite different names*

## Comparing `lense/lense/cglense.py` & `lense/backend/cglense.py`

 * *Files identical despite different names*

## Comparing `lense/lense/csv_engine.py` & `lense/backend/csv_engine.py`

 * *Files identical despite different names*

## Comparing `lense/lense/error_handling.py` & `lense/backend/error_handling.py`

 * *Files identical despite different names*

## Comparing `lense/lense/loader.py` & `lense/backend/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import pathlib
 import warnings
 from llama_index.readers.file import PyMuPDFReader
-from lense.lense.error_handling import *
-from lense.lense.replace_file import *
+from lense.backend.error_handling import *
+from lense.backend.replace_file import *
 
 
 def load_csv(file_path):
     try:
         data = pd.read_csv(file_path)
         return data
     except Exception as e:
```

## Comparing `lense/lense/qna_engine.py` & `lense/backend/qna_engine.py`

 * *Files identical despite different names*

## Comparing `lense/lense/replace_file.py` & `lense/backend/replace_file.py`

 * *Files identical despite different names*

## Comparing `lense-0.0.5.dist-info/METADATA` & `lense-0.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lense
-Version: 0.0.5
+Version: 0.0.6
 Requires-Dist: pandas ==2.2.2
 Requires-Dist: PyPDF2 ==3.0.1
 Requires-Dist: python-docx ==1.1.0
 Requires-Dist: python-pptx ==0.6.23
 Requires-Dist: llama-index ==0.10.29
 Requires-Dist: llama-index.llms.azure-openai ==0.1.5
 Requires-Dist: llama-index.embeddings.azure-openai ==0.1.6
```

