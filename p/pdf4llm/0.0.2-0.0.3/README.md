# Comparing `tmp/pdf4llm-0.0.2.tar.gz` & `tmp/pdf4llm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.2.tar", last modified: Tue Apr 23 08:11:07 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.3.tar", last modified: Tue Apr 23 08:41:25 2024, max compression
```

## Comparing `pdf4llm-0.0.2.tar` & `pdf4llm-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.082424 pdf4llm-0.0.2/
--rw-rw-rw-   0        0        0    35184 2024-03-21 16:34:42.000000 pdf4llm-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2445 2024-04-23 08:11:07.081423 pdf4llm-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1910 2024-04-23 04:27:37.000000 pdf4llm-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.068268 pdf4llm-0.0.2/pdf4llm/
--rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.2/pdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.080424 pdf4llm-0.0.2/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     2445 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 08:11:07.082424 pdf4llm-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      890 2024-04-23 08:10:59.000000 pdf4llm-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:41:25.229900 pdf4llm-0.0.3/
+-rw-rw-rw-   0        0        0     2493 2024-04-23 08:41:25.228900 pdf4llm-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 08:41:25.227896 pdf4llm-0.0.3/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     2493 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:41:25.229900 pdf4llm-0.0.3/setup.cfg
```

### Comparing `pdf4llm-0.0.2/PKG-INFO` & `pdf4llm-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: pymupdf>=1.24.2
 
 # Using PyMuPDF in an RAG (Retrieval-Augmented Generation) Chatbot Environment
 
 This repository contains examples showing how PyMuPDF can be used as a data feed for RAG-based chatbots.
 
 Examples include scripts that start chatbots - either as simple CLI programs in REPL mode or browser-based GUIs.
@@ -39,15 +38,14 @@
 $ pip install -U pdf4llm
 ```
 
 Then in your script do
 
 ```python
 import pdf4llm
-import fitz
 
-doc = fitz.open("input.pdf")
-
-md_text = pdf4llm.to_markdown(doc)
+md_text = pdf4llm.to_markdown("input.pdf", pages=page_numbers)
 
 # work with the markdown text
 ```
+
+Instead of the filename string as above, you can also provide a PyMuPDF `Document`.
```

### Comparing `pdf4llm-0.0.2/pdf4llm.egg-info/PKG-INFO` & `pdf4llm-0.0.3/pdf4llm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: pymupdf>=1.24.2
 
 # Using PyMuPDF in an RAG (Retrieval-Augmented Generation) Chatbot Environment
 
 This repository contains examples showing how PyMuPDF can be used as a data feed for RAG-based chatbots.
 
 Examples include scripts that start chatbots - either as simple CLI programs in REPL mode or browser-based GUIs.
@@ -39,15 +38,14 @@
 $ pip install -U pdf4llm
 ```
 
 Then in your script do
 
 ```python
 import pdf4llm
-import fitz
 
-doc = fitz.open("input.pdf")
-
-md_text = pdf4llm.to_markdown(doc)
+md_text = pdf4llm.to_markdown("input.pdf", pages=page_numbers)
 
 # work with the markdown text
 ```
+
+Instead of the filename string as above, you can also provide a PyMuPDF `Document`.
```

