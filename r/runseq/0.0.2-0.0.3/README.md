# Comparing `tmp/runseq-0.0.2.tar.gz` & `tmp/runseq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runseq-0.0.2.tar", last modified: Tue Apr 23 15:03:31 2024, max compression
+gzip compressed data, was "runseq-0.0.3.tar", last modified: Tue Apr 23 15:31:20 2024, max compression
```

## Comparing `runseq-0.0.2.tar` & `runseq-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:03:31.440751 runseq-0.0.2/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.0.2/LICENSE
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      195 2024-04-23 15:03:31.440751 runseq-0.0.2/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     1425 2024-04-23 15:02:25.000000 runseq-0.0.2/README.md
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:03:31.440751 runseq-0.0.2/runseq.egg-info/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      195 2024-04-23 15:03:31.000000 runseq-0.0.2/runseq.egg-info/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      191 2024-04-23 15:03:31.000000 runseq-0.0.2/runseq.egg-info/SOURCES.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-23 15:03:31.000000 runseq-0.0.2/runseq.egg-info/dependency_links.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-23 15:03:31.000000 runseq-0.0.2/runseq.egg-info/entry_points.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-23 15:03:31.000000 runseq-0.0.2/runseq.egg-info/top_level.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     4375 2024-04-23 14:46:16.000000 runseq-0.0.2/runseq.py
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:03:31.440751 runseq-0.0.2/setup.cfg
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      600 2024-04-23 15:03:18.000000 runseq-0.0.2/setup.py
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:31:20.788134 runseq-0.0.3/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.0.3/LICENSE
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    42296 2024-04-23 15:31:20.788134 runseq-0.0.3/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     1425 2024-04-23 15:05:01.000000 runseq-0.0.3/README.md
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-04-23 15:31:18.000000 runseq-0.0.3/pyproject.toml
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:31:20.788134 runseq-0.0.3/runseq.egg-info/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    42296 2024-04-23 15:31:20.000000 runseq-0.0.3/runseq.egg-info/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-04-23 15:31:20.000000 runseq-0.0.3/runseq.egg-info/SOURCES.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-23 15:31:20.000000 runseq-0.0.3/runseq.egg-info/dependency_links.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-23 15:31:20.000000 runseq-0.0.3/runseq.egg-info/entry_points.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-23 15:31:20.000000 runseq-0.0.3/runseq.egg-info/top_level.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     4445 2024-04-23 15:15:09.000000 runseq-0.0.3/runseq.py
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:31:20.788134 runseq-0.0.3/setup.cfg
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.0.3/setup.py
```

### Comparing `runseq-0.0.2/LICENSE` & `runseq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runseq-0.0.2/README.md` & `runseq-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `runseq-0.0.2/runseq.py` & `runseq-0.0.3/runseq.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import sys
 import time
 
 from datetime import datetime
 
 
 __version__ = "0.0.2"
+__author__ = "Luís Gomes"
+__author_email__ = "luismsgomes@gmail.com"
 
 
 DB_PATH = os.environ.get("RUNSEQ_DB", "runseq.sqlite3")
 
 
 def db_connect():
     con = sqlite3.connect(DB_PATH)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

