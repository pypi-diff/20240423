# Comparing `tmp/simple-wikiparser-0.0.0.tar.gz` & `tmp/simple-wikiparser-0.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wikiparser-0.0.0.tar", last modified: Mon Apr 22 12:28:04 2024, max compression
+gzip compressed data, was "simple-wikiparser-0.0.0a0.tar", last modified: Tue Apr 23 05:28:09 2024, max compression
```

## Comparing `simple-wikiparser-0.0.0.tar` & `simple-wikiparser-0.0.0a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:04.115193 simple-wikiparser-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 12:27:45.000000 simple-wikiparser-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-22 12:28:04.115193 simple-wikiparser-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 12:27:45.000000 simple-wikiparser-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:28:04.115193 simple-wikiparser-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 12:27:45.000000 simple-wikiparser-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:04.115193 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-22 12:28:04.000000 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 12:28:04.000000 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:28:04.000000 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 12:28:04.000000 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 12:28:04.000000 simple-wikiparser-0.0.0/simple_wikiparser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:04.115193 simple-wikiparser-0.0.0/wikiparser/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:27:45.000000 simple-wikiparser-0.0.0/wikiparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-22 12:27:45.000000 simple-wikiparser-0.0.0/wikiparser/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:28:09.242617 simple-wikiparser-0.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 05:27:47.000000 simple-wikiparser-0.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 05:28:09.242617 simple-wikiparser-0.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-23 05:27:47.000000 simple-wikiparser-0.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 05:28:09.242617 simple-wikiparser-0.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 05:27:47.000000 simple-wikiparser-0.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:28:09.242617 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 05:28:09.000000 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 05:28:09.000000 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 05:28:09.000000 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 05:28:09.000000 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 05:28:09.000000 simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:28:09.242617 simple-wikiparser-0.0.0a0/wikiparser/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 05:27:47.000000 simple-wikiparser-0.0.0a0/wikiparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-23 05:27:47.000000 simple-wikiparser-0.0.0a0/wikiparser/core.py
```

### Comparing `simple-wikiparser-0.0.0/LICENSE` & `simple-wikiparser-0.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-wikiparser-0.0.0/PKG-INFO` & `simple-wikiparser-0.0.0a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wikiparser
-Version: 0.0.0
+Version: 0.0.0a0
 Summary: A simple Wikipedia parser
 Home-page: https://github.com/biswajit2903/SimpleWikiParser
 Author: Biswajit Satapathy
 Author-email: biswajit2902@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 # SimpleWikiParser
 An Simplified Wiki Data Parser
 
 ## Installation
 ```bash
-pip install git+https://github.com/Biswajit2902/SimpleWikiParser.git
+pip install simple-wikiparser
 ```
 
 ## Usage:
 ```python
 from wikiparser.core import WikiMediaDumpParser
 
 # initialise Parser for a language (say Hindi)
```

### Comparing `simple-wikiparser-0.0.0/setup.py` & `simple-wikiparser-0.0.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,9 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.8',
+    include_package_data=True
 )
```

### Comparing `simple-wikiparser-0.0.0/simple_wikiparser.egg-info/PKG-INFO` & `simple-wikiparser-0.0.0a0/simple_wikiparser.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wikiparser
-Version: 0.0.0
+Version: 0.0.0a0
 Summary: A simple Wikipedia parser
 Home-page: https://github.com/biswajit2903/SimpleWikiParser
 Author: Biswajit Satapathy
 Author-email: biswajit2902@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 # SimpleWikiParser
 An Simplified Wiki Data Parser
 
 ## Installation
 ```bash
-pip install git+https://github.com/Biswajit2902/SimpleWikiParser.git
+pip install simple-wikiparser
 ```
 
 ## Usage:
 ```python
 from wikiparser.core import WikiMediaDumpParser
 
 # initialise Parser for a language (say Hindi)
```

### Comparing `simple-wikiparser-0.0.0/wikiparser/core.py` & `simple-wikiparser-0.0.0a0/wikiparser/core.py`

 * *Files identical despite different names*

