# Comparing `tmp/lense-0.0.4-py3-none-any.whl.zip` & `tmp/lense-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9941 bytes, number of entries: 14
+Zip file size: 9943 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-22 06:00 lense/__init__.py
--rw-rw-rw-  2.0 fat     6557 b- defN 24-Apr-22 09:09 lense/app.py
+-rw-rw-rw-  2.0 fat     6527 b- defN 24-Apr-23 07:49 lense/app.py
 -rw-rw-rw-  2.0 fat     3290 b- defN 24-Apr-22 07:32 lense/lense/SQL_engine.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-22 06:59 lense/lense/__init__.py
 -rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-22 07:20 lense/lense/cglense.py
 -rw-rw-rw-  2.0 fat     5836 b- defN 24-Apr-22 07:22 lense/lense/csv_engine.py
 -rw-rw-rw-  2.0 fat     4694 b- defN 24-Apr-22 07:24 lense/lense/error_handling.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-22 09:10 lense/lense/loader.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 24-Apr-23 07:49 lense/lense/loader.py
 -rw-rw-rw-  2.0 fat     2464 b- defN 24-Apr-22 07:28 lense/lense/qna_engine.py
 -rw-rw-rw-  2.0 fat     3336 b- defN 24-Apr-22 07:31 lense/lense/replace_file.py
--rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 07:46 lense-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 07:46 lense-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 07:46 lense-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1079 b- defN 24-Apr-23 07:46 lense-0.0.4.dist-info/RECORD
-14 files, 30551 bytes uncompressed, 8163 bytes compressed:  73.3%
+-rw-rw-rw-  2.0 fat      930 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1079 b- defN 24-Apr-23 07:50 lense-0.0.5.dist-info/RECORD
+14 files, 30509 bytes uncompressed, 8165 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: lense/lense/qna_engine.py
 Comment: 
 
 Filename: lense/lense/replace_file.py
 Comment: 
 
-Filename: lense-0.0.4.dist-info/METADATA
+Filename: lense-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: lense-0.0.4.dist-info/WHEEL
+Filename: lense-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: lense-0.0.4.dist-info/top_level.txt
+Filename: lense-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lense-0.0.4.dist-info/RECORD
+Filename: lense-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lense/app.py

```diff
@@ -1,17 +1,17 @@
 #from loader import load_document
-from lense.lense.lense.qna_engine import *
-from lense.lense.lense.SQL_engine import *
-from lense.lense.lense.csv_engine import *
+from lense.lense.qna_engine import *
+from lense.lense.SQL_engine import *
+from lense.lense.csv_engine import *
 from fastapi import FastAPI, File, UploadFile, Form
 from enum import Enum
-from lense.lense.lense.qna_engine import embed_and_run_openai, embed_and_run_azureopenai, embed_and_run_mistral
+from lense.lense.qna_engine import embed_and_run_openai, embed_and_run_azureopenai, embed_and_run_mistral
 import shutil
 import os
-from lense.lense.lense.loader import load_document
+from lense.lense.loader import load_document
 from fastapi import FastAPI, Request ,APIRouter
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 import uvicorn
 
 
 app = FastAPI()
```

## lense/lense/loader.py

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import pathlib
 import warnings
 from llama_index.readers.file import PyMuPDFReader
-from lense.lense.lense.error_handling import *
-from lense.lense.lense.replace_file import *
+from lense.lense.error_handling import *
+from lense.lense.replace_file import *
 
 
 def load_csv(file_path):
     try:
         data = pd.read_csv(file_path)
         return data
     except Exception as e:
```

## Comparing `lense-0.0.4.dist-info/METADATA` & `lense-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lense
-Version: 0.0.4
+Version: 0.0.5
 Requires-Dist: pandas ==2.2.2
 Requires-Dist: PyPDF2 ==3.0.1
 Requires-Dist: python-docx ==1.1.0
 Requires-Dist: python-pptx ==0.6.23
 Requires-Dist: llama-index ==0.10.29
 Requires-Dist: llama-index.llms.azure-openai ==0.1.5
 Requires-Dist: llama-index.embeddings.azure-openai ==0.1.6
```

## Comparing `lense-0.0.4.dist-info/RECORD` & `lense-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 lense/__init__.py,sha256=5rivs2U5ia9uXArxLc1H8FyzIZXtDjxp_vsZsUEDo60,22
-lense/app.py,sha256=M3xoSyNfRNDCRbdEtG8089zTLdpEOVMrPM7WavJe1zQ,6557
+lense/app.py,sha256=MlzIUGlwCYkrHWTfTTUVirgcNmvRtLB7SeTMFeIF0ug,6527
 lense/lense/SQL_engine.py,sha256=Gzs7MM3n-xACgZ6sAUbRZxdecvcP819YBFNhiNy8020,3290
 lense/lense/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lense/lense/cglense.py,sha256=nba7Qa0B64U1RzhFenAOiFfarNS5qYSt0IPeqpHhSWA,1173
 lense/lense/csv_engine.py,sha256=id-MVVsjD2KZlB8Q0gvols1db2Ot5t7K1HemEDx_gN8,5836
 lense/lense/error_handling.py,sha256=HjB1eD-2jwhC7-rwvUc6CtYICjinKnMKop4DheUQOM4,4694
-lense/lense/loader.py,sha256=EJHCtuFtaw3ezSxmQdlSWPaInHUMzceMWda-duw9238,1072
+lense/lense/loader.py,sha256=Uqy-pMKnY7Pa7PAzSytIfD5mxOys8RAjJ_jYxuB8_Sk,1060
 lense/lense/qna_engine.py,sha256=VZkoMp-jqitYdWOsoctmeN1ApBE5cxyGJ2IHI6Wz994,2464
 lense/lense/replace_file.py,sha256=-DzKIrFXiKwhMZAPW7GSfDIhV9FGB7yhOqp3OqlS7eE,3336
-lense-0.0.4.dist-info/METADATA,sha256=3YcrcL3CJvGYvNJPRWzSB2QgioAnMAe-wv5S8ifAOMY,930
-lense-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-lense-0.0.4.dist-info/top_level.txt,sha256=iyP2ZFtpvgpecDSV53lznPmRGjO3FUFAnNUkUTRbxIg,6
-lense-0.0.4.dist-info/RECORD,,
+lense-0.0.5.dist-info/METADATA,sha256=rmA1B1g-_wG46takBjBRWRKumKjcEPuxuAVT3YIvQ80,930
+lense-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+lense-0.0.5.dist-info/top_level.txt,sha256=iyP2ZFtpvgpecDSV53lznPmRGjO3FUFAnNUkUTRbxIg,6
+lense-0.0.5.dist-info/RECORD,,
```

