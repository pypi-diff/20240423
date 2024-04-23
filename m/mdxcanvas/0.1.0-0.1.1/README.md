# Comparing `tmp/mdxcanvas-0.1.0.tar.gz` & `tmp/mdxcanvas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.0.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.1.tar", max compression
```

## Comparing `mdxcanvas-0.1.0.tar` & `mdxcanvas-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.0/LICENSE
--rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.0/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    20889 2024-04-22 22:07:08.576608 mdxcanvas-0.1.0/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0      908 2024-02-23 20:06:54.416736 mdxcanvas-0.1.0/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3392 2024-04-22 22:07:08.576705 mdxcanvas-0.1.0/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.0/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.0/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25486 2024-04-22 22:07:08.577304 mdxcanvas-0.1.0/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.0/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.0/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15308 2024-04-22 22:07:08.577804 mdxcanvas-0.1.0/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-04-22 22:08:25.240353 mdxcanvas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.1/LICENSE
+-rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.1/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    20788 2024-04-23 21:52:37.729116 mdxcanvas-0.1.1/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0      914 2024-04-23 21:43:27.025380 mdxcanvas-0.1.1/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3392 2024-04-22 22:07:08.576705 mdxcanvas-0.1.1/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.1/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.1/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25486 2024-04-22 22:07:08.577304 mdxcanvas-0.1.1/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.1/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.1/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15308 2024-04-22 22:07:08.577804 mdxcanvas-0.1.1/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-04-23 21:52:48.699614 mdxcanvas-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.1/PKG-INFO
```

### Comparing `mdxcanvas-0.1.0/LICENSE` & `mdxcanvas-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.1/mdxcanvas/canvas_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-import random
-import re
-from datetime import datetime
 import json
-import os
+import random
 import textwrap
 import uuid
+from datetime import datetime
+from pathlib import Path
 
-import pygments
-
-import argparse
-from xml.etree import ElementTree as etree
-
+import markdown as md
 import pytz
+from bs4 import BeautifulSoup
 from canvasapi import Canvas
 from canvasapi.assignment import Assignment
-
-from canvasapi.quiz import Quiz
 from canvasapi.course import Course
 from canvasapi.module import Module
-
-import markdown as md
+from canvasapi.quiz import Quiz
 from markdown.extensions.codehilite import makeExtension as makeCodehiliteExtension
 
-from pathlib import Path
-from bs4 import BeautifulSoup
-
 from jinja_parser import process_jinja
-
 from .extensions import BlackInlineCodeExtension
 from .parser import DocumentParser, make_iso
 from .yaml_parser import DocumentWalker, parse_yaml
 
 
 def readfile(filepath: Path):
     with open(filepath) as file:
```

### Comparing `mdxcanvas-0.1.0/mdxcanvas/deploy.py` & `mdxcanvas-0.1.1/mdxcanvas/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from pathlib import Path
-from mdxcanvas import post_document, get_course
+from .canvas_creator import post_document, get_course
 import json
 import os
 
 
 def main(api_url, api_token, course_id, time_zone: str, file_path: Path):
     print("-" * 50 + "\nCanvas MDX\n" + "-" * 50)
```

### Comparing `mdxcanvas-0.1.0/mdxcanvas/document_schema.py` & `mdxcanvas-0.1.1/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/extensions.py` & `mdxcanvas-0.1.1/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.1.1/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/parser.py` & `mdxcanvas-0.1.1/mdxcanvas/parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/question_schema.py` & `mdxcanvas-0.1.1/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/templating.py` & `mdxcanvas-0.1.1/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.1.1/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.0/pyproject.toml` & `mdxcanvas-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.0/PKG-INFO` & `mdxcanvas-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

