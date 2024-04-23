# Comparing `tmp/pdf4llm-0.0.1.tar.gz` & `tmp/pdf4llm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.1.tar", last modified: Mon Apr 22 23:26:31 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.2.tar", last modified: Tue Apr 23 08:11:07 2024, max compression
```

## Comparing `pdf4llm-0.0.1.tar` & `pdf4llm-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 23:26:31.405989 pdf4llm-0.0.1/
--rw-rw-rw-   0        0        0    35184 2024-03-21 16:34:42.000000 pdf4llm-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2215 2024-04-22 23:26:31.404989 pdf4llm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1680 2024-04-22 16:48:39.000000 pdf4llm-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 23:26:31.379969 pdf4llm-0.0.1/pdf4llm/
--rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.1/pdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:26:31.380968 pdf4llm-0.0.1/pdf4llm/helpers/
--rw-rw-rw-   0        0        0     1592 2024-04-08 15:51:31.000000 pdf4llm-0.0.1/pdf4llm/helpers/README.md
--rw-rw-rw-   0        0        0    13715 2024-04-08 17:18:45.000000 pdf4llm-0.0.1/pdf4llm/helpers/pymupdf_rag.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:26:31.403996 pdf4llm-0.0.1/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     2215 2024-04-22 23:26:31.000000 pdf4llm-0.0.1/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-22 23:26:31.000000 pdf4llm-0.0.1/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 23:26:31.000000 pdf4llm-0.0.1/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 23:26:31.000000 pdf4llm-0.0.1/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 23:26:31.000000 pdf4llm-0.0.1/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 23:26:31.405989 pdf4llm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1394 2024-04-22 23:06:03.000000 pdf4llm-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.082424 pdf4llm-0.0.2/
+-rw-rw-rw-   0        0        0    35184 2024-03-21 16:34:42.000000 pdf4llm-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2445 2024-04-23 08:11:07.081423 pdf4llm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1910 2024-04-23 04:27:37.000000 pdf4llm-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.068268 pdf4llm-0.0.2/pdf4llm/
+-rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.2/pdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:11:07.080424 pdf4llm-0.0.2/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     2445 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 08:11:06.000000 pdf4llm-0.0.2/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:11:07.082424 pdf4llm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      890 2024-04-23 08:10:59.000000 pdf4llm-0.0.2/setup.py
```

### Comparing `pdf4llm-0.0.1/LICENSE` & `pdf4llm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf4llm-0.0.1/PKG-INFO` & `pdf4llm-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,12 +25,29 @@
 1. **Extract Text**: Use PyMuPDF to extract text from one or more pages from one or more PDFs. Depending on the specific requirement this may be all text or only text contained in tables, the Table of Contents, etc.
 This will generally be implemented as one or more Python functions called by any of the following events - which implement the actual chatbot functionality.
 2. **Indexing the Extracted Text**: Index the extracted text for efficient retrieval. This index will act as the knowledge base for the chatbot.
 3. **Query Processing**: When a user asks a question, process the query to determine the key information needed for a response.
 4. **Retrieving Relevant Information**: Search your indexed knowledge base for the most relevant pieces of information related to the user's query.
 5. **Generating a Response**: Use a generative model to generate a response based on the retrieved information.
 
+# Installation
+
 As a specialty, folder "helpers" contains a script that is capable to convert PDF pages into **_text strings in Markdown format_**, which includes standard text as well as table-based text in a consistent and integrated view. This is especially important in RAG environments.
 
-# Installation
+There exists a Python package on PyPI [pdf4llm](https://pypi.org/project/pdf4llm/) which provides easy access to this script:
+
+```bash
+$ pip install -U pdf4llm
+```
+
+Then in your script do
+
+```python
+import pdf4llm
+import fitz
+
+doc = fitz.open("input.pdf")
+
+md_text = pdf4llm.to_markdown(doc)
 
-The repository can be installed under the name "pdf4llm" (PDF for LLM) in the usual way `pip install -U pdf4llm`.
+# work with the markdown text
+```
```

### Comparing `pdf4llm-0.0.1/README.md` & `pdf4llm-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,12 +8,29 @@
 1. **Extract Text**: Use PyMuPDF to extract text from one or more pages from one or more PDFs. Depending on the specific requirement this may be all text or only text contained in tables, the Table of Contents, etc.
 This will generally be implemented as one or more Python functions called by any of the following events - which implement the actual chatbot functionality.
 2. **Indexing the Extracted Text**: Index the extracted text for efficient retrieval. This index will act as the knowledge base for the chatbot.
 3. **Query Processing**: When a user asks a question, process the query to determine the key information needed for a response.
 4. **Retrieving Relevant Information**: Search your indexed knowledge base for the most relevant pieces of information related to the user's query.
 5. **Generating a Response**: Use a generative model to generate a response based on the retrieved information.
 
+# Installation
+
 As a specialty, folder "helpers" contains a script that is capable to convert PDF pages into **_text strings in Markdown format_**, which includes standard text as well as table-based text in a consistent and integrated view. This is especially important in RAG environments.
 
-# Installation
+There exists a Python package on PyPI [pdf4llm](https://pypi.org/project/pdf4llm/) which provides easy access to this script:
+
+```bash
+$ pip install -U pdf4llm
+```
+
+Then in your script do
+
+```python
+import pdf4llm
+import fitz
+
+doc = fitz.open("input.pdf")
+
+md_text = pdf4llm.to_markdown(doc)
 
-The repository can be installed under the name "pdf4llm" (PDF for LLM) in the usual way `pip install -U pdf4llm`.
+# work with the markdown text
+```
```

### Comparing `pdf4llm-0.0.1/pdf4llm.egg-info/PKG-INFO` & `pdf4llm-0.0.2/pdf4llm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf4llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,12 +25,29 @@
 1. **Extract Text**: Use PyMuPDF to extract text from one or more pages from one or more PDFs. Depending on the specific requirement this may be all text or only text contained in tables, the Table of Contents, etc.
 This will generally be implemented as one or more Python functions called by any of the following events - which implement the actual chatbot functionality.
 2. **Indexing the Extracted Text**: Index the extracted text for efficient retrieval. This index will act as the knowledge base for the chatbot.
 3. **Query Processing**: When a user asks a question, process the query to determine the key information needed for a response.
 4. **Retrieving Relevant Information**: Search your indexed knowledge base for the most relevant pieces of information related to the user's query.
 5. **Generating a Response**: Use a generative model to generate a response based on the retrieved information.
 
+# Installation
+
 As a specialty, folder "helpers" contains a script that is capable to convert PDF pages into **_text strings in Markdown format_**, which includes standard text as well as table-based text in a consistent and integrated view. This is especially important in RAG environments.
 
-# Installation
+There exists a Python package on PyPI [pdf4llm](https://pypi.org/project/pdf4llm/) which provides easy access to this script:
+
+```bash
+$ pip install -U pdf4llm
+```
+
+Then in your script do
+
+```python
+import pdf4llm
+import fitz
+
+doc = fitz.open("input.pdf")
+
+md_text = pdf4llm.to_markdown(doc)
 
-The repository can be installed under the name "pdf4llm" (PDF for LLM) in the usual way `pip install -U pdf4llm`.
+# work with the markdown text
+```
```

### Comparing `pdf4llm-0.0.1/setup.py` & `pdf4llm-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,37 +10,22 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
 requires = ["pymupdf>=1.24.2"]
-print(setuptools.find_packages())
+
 setuptools.setup(
     name="pdf4llm",
-    version="0.0.1",
+    version="0.0.2",
     author="Artifex",
     author_email="support@artifex.com",
     description="PyMuPDF Utilities for LLM/RAG",
     packages=setuptools.find_packages(),
-    package_dir={"": "."},
-    package_data={
-        "pdf4llm": [
-            "LICENSE",
-            "helpers/input.pdf",
-            "helpers/input2.pdf",
-            "helpers/pymupdf_rag.py",
-            "helpers/README.md",
-            "country-capitals/country-capitals.py",
-            "country-capitals/national-capitals.pdf",
-            "country-capitals/README.md",
-            "GUI/browser-app.py",
-            "GUI/README.md",
-        ]
-    },
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
     license="GNU AFFERO GPL 3.0",
     url="https://github.com/pymupdf/RAG",
     classifiers=classifiers,
     project_urls={},
```

