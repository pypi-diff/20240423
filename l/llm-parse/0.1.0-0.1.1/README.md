# Comparing `tmp/llm_parse-0.1.0.tar.gz` & `tmp/llm_parse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_parse-0.1.0.tar", max compression
+gzip compressed data, was "llm_parse-0.1.1.tar", max compression
```

## Comparing `llm_parse-0.1.0.tar` & `llm_parse-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-19 15:47:45.995075 llm_parse-0.1.0/LICENSE
--rw-r--r--   0        0        0     1382 2024-04-22 15:12:40.636191 llm_parse-0.1.0/README.md
--rw-r--r--   0        0        0      244 2024-04-22 15:00:37.104345 llm_parse-0.1.0/llm_parse/__init__.py
--rw-r--r--   0        0        0      354 2024-04-22 14:53:02.976941 llm_parse-0.1.0/llm_parse/base.py
--rw-r--r--   0        0        0     1225 2024-04-22 15:17:09.301494 llm_parse-0.1.0/llm_parse/llamaparse_parser.py
--rw-r--r--   0        0        0    12577 2024-04-22 10:44:23.490249 llm_parse-0.1.0/llm_parse/pdf_2_md_parser.py
--rw-r--r--   0        0        0     1585 2024-04-21 02:28:18.395369 llm_parse-0.1.0/llm_parse/pdf_2_text_parser.py
--rw-r--r--   0        0        0     4252 2024-04-22 10:42:53.827780 llm_parse-0.1.0/llm_parse/utils.py
--rw-r--r--   0        0        0      471 2024-04-22 13:49:13.104406 llm_parse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 llm_parse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-19 15:47:45.995075 llm_parse-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1382 2024-04-22 15:12:40.636191 llm_parse-0.1.1/README.md
+-rw-r--r--   0        0        0      244 2024-04-22 15:00:37.104345 llm_parse-0.1.1/llm_parse/__init__.py
+-rw-r--r--   0        0        0      354 2024-04-22 14:53:02.976941 llm_parse-0.1.1/llm_parse/base.py
+-rw-r--r--   0        0        0     1225 2024-04-22 15:17:09.301494 llm_parse-0.1.1/llm_parse/llamaparse_parser.py
+-rw-r--r--   0        0        0    12567 2024-04-23 02:01:16.137883 llm_parse-0.1.1/llm_parse/pdf_2_md_parser.py
+-rw-r--r--   0        0        0     1585 2024-04-21 02:28:18.395369 llm_parse-0.1.1/llm_parse/pdf_2_text_parser.py
+-rw-r--r--   0        0        0     4252 2024-04-22 10:42:53.827780 llm_parse-0.1.1/llm_parse/utils.py
+-rw-r--r--   0        0        0      471 2024-04-23 02:05:57.926797 llm_parse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 llm_parse-0.1.1/PKG-INFO
```

### Comparing `llm_parse-0.1.0/LICENSE` & `llm_parse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.0/README.md` & `llm_parse-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.0/llm_parse/llamaparse_parser.py` & `llm_parse-0.1.1/llm_parse/llamaparse_parser.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.0/llm_parse/pdf_2_md_parser.py` & `llm_parse-0.1.1/llm_parse/pdf_2_md_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 import string
 
 import fitz
 
 from llm_parse.base import BaseParser
 from llm_parse.utils import (
     compress_multiline,
```

### Comparing `llm_parse-0.1.0/llm_parse/pdf_2_text_parser.py` & `llm_parse-0.1.1/llm_parse/pdf_2_text_parser.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.0/llm_parse/utils.py` & `llm_parse-0.1.1/llm_parse/utils.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.0/PKG-INFO` & `llm_parse-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: llm-parse
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parse data from documents optimised for downstream llm tasks.
 License: MIT
 Author: tanchangsheng
 Author-email: tancs1994@hotmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-parse (>=0.4.1,<0.5.0)
 Requires-Dist: pdfplumber (>=0.11.0,<0.12.0)
 Requires-Dist: pymupdf (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
```

