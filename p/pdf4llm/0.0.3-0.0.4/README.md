# Comparing `tmp/pdf4llm-0.0.3.tar.gz` & `tmp/pdf4llm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.3.tar", last modified: Tue Apr 23 08:41:25 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.4.tar", last modified: Tue Apr 23 09:00:03 2024, max compression
```

## Comparing `pdf4llm-0.0.3.tar` & `pdf4llm-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:41:25.229900 pdf4llm-0.0.3/
--rw-rw-rw-   0        0        0     2493 2024-04-23 08:41:25.228900 pdf4llm-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 08:41:25.227896 pdf4llm-0.0.3/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     2493 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:41:25.000000 pdf4llm-0.0.3/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 08:41:25.229900 pdf4llm-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 09:00:03.420924 pdf4llm-0.0.4/
+-rw-rw-rw-   0        0        0    35184 2024-03-21 16:34:42.000000 pdf4llm-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2516 2024-04-23 09:00:03.419925 pdf4llm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1979 2024-04-23 08:21:48.000000 pdf4llm-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 09:00:03.401970 pdf4llm-0.0.4/pdf4llm/
+-rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.4/pdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:00:03.418924 pdf4llm-0.0.4/pdf4llm/helpers/
+-rw-rw-rw-   0        0        0    13775 2024-04-23 08:06:26.000000 pdf4llm-0.0.4/pdf4llm/helpers/pymupdf_rag.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:00:03.417919 pdf4llm-0.0.4/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     2516 2024-04-23 09:00:03.000000 pdf4llm-0.0.4/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-23 09:00:03.000000 pdf4llm-0.0.4/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:00:03.000000 pdf4llm-0.0.4/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 09:00:03.000000 pdf4llm-0.0.4/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 09:00:03.000000 pdf4llm-0.0.4/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 09:00:03.420924 pdf4llm-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      980 2024-04-23 08:59:34.000000 pdf4llm-0.0.4/setup.py
```

### Comparing `pdf4llm-0.0.3/PKG-INFO` & `pdf4llm-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.3
+Version: 0.0.4
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
+License-File: LICENSE
 Requires-Dist: pymupdf>=1.24.2
 
 # Using PyMuPDF in an RAG (Retrieval-Augmented Generation) Chatbot Environment
 
 This repository contains examples showing how PyMuPDF can be used as a data feed for RAG-based chatbots.
 
 Examples include scripts that start chatbots - either as simple CLI programs in REPL mode or browser-based GUIs.
```

### Comparing `pdf4llm-0.0.3/pdf4llm.egg-info/PKG-INFO` & `pdf4llm-0.0.4/pdf4llm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.3
+Version: 0.0.4
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
+License-File: LICENSE
 Requires-Dist: pymupdf>=1.24.2
 
 # Using PyMuPDF in an RAG (Retrieval-Augmented Generation) Chatbot Environment
 
 This repository contains examples showing how PyMuPDF can be used as a data feed for RAG-based chatbots.
 
 Examples include scripts that start chatbots - either as simple CLI programs in REPL mode or browser-based GUIs.
```

