# Comparing `tmp/datafog-3.0.0b2.tar.gz` & `tmp/datafog-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.0.0b2.tar", last modified: Mon Apr 22 15:53:14 2024, max compression
+gzip compressed data, was "datafog-3.0.0b3.tar", last modified: Mon Apr 22 19:01:09 2024, max compression
```

## Comparing `datafog-3.0.0b2.tar` & `datafog-3.0.0b3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 15:53:14.028277 datafog-3.0.0b2/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-21 22:55:54.000000 datafog-3.0.0b2/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 15:53:14.028049 datafog-3.0.0b2/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-21 22:55:54.000000 datafog-3.0.0b2/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-22 15:53:14.028327 datafog-3.0.0b2/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1679 2024-04-22 15:51:31.000000 datafog-3.0.0b2/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 15:53:14.025024 datafog-3.0.0b2/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 15:53:14.026484 datafog-3.0.0b2/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       29 2024-04-22 15:51:35.000000 datafog-3.0.0b2/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      978 2024-04-21 23:54:42.000000 datafog-3.0.0b2/src/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2101 2024-04-21 23:54:11.000000 datafog-3.0.0b2/src/datafog/models.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      318 2024-04-21 23:54:42.000000 datafog-3.0.0b2/src/datafog/utils.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 15:53:14.027759 datafog-3.0.0b2/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 15:53:13.000000 datafog-3.0.0b2/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      326 2024-04-22 15:53:13.000000 datafog-3.0.0b2/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-22 15:53:13.000000 datafog-3.0.0b2/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       76 2024-04-22 15:53:13.000000 datafog-3.0.0b2/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       13 2024-04-22 15:53:13.000000 datafog-3.0.0b2/src/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      970 2024-04-21 23:54:11.000000 datafog-3.0.0b2/src/test.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 15:53:14.027471 datafog-3.0.0b2/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)      934 2024-04-21 23:54:11.000000 datafog-3.0.0b2/tests/test_datafog.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.874369 datafog-3.0.0b3/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-21 22:55:54.000000 datafog-3.0.0b3/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 19:01:09.874126 datafog-3.0.0b3/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-21 22:55:54.000000 datafog-3.0.0b3/README.md
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-22 19:01:09.874419 datafog-3.0.0b3/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1679 2024-04-22 19:00:14.000000 datafog-3.0.0b3/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.871244 datafog-3.0.0b3/src/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.872166 datafog-3.0.0b3/src/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       29 2024-04-22 19:00:06.000000 datafog-3.0.0b3/src/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1929 2024-04-22 18:52:58.000000 datafog-3.0.0b3/src/datafog/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873304 datafog-3.0.0b3/src/datafog/image_processors/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       46 2024-04-22 17:55:38.000000 datafog-3.0.0b3/src/datafog/image_processors/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4216 2024-04-22 18:57:45.000000 datafog-3.0.0b3/src/datafog/image_processors/donut_model.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2101 2024-04-21 23:54:11.000000 datafog-3.0.0b3/src/datafog/models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      318 2024-04-21 23:54:42.000000 datafog-3.0.0b3/src/datafog/utils.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873752 datafog-3.0.0b3/src/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      411 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       76 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       13 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2044 2024-04-22 18:55:04.000000 datafog-3.0.0b3/src/test.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873532 datafog-3.0.0b3/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      934 2024-04-21 23:54:11.000000 datafog-3.0.0b3/tests/test_datafog.py
```

### Comparing `datafog-3.0.0b2/LICENSE` & `datafog-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b2/PKG-INFO` & `datafog-3.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b2 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b3 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.0.0b2/README.md` & `datafog-3.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b2/setup.py` & `datafog-3.0.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.0.0-beta.2"
+    return "3.0.0-beta.3"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.0.0b2/src/datafog/models.py` & `datafog-3.0.0b3/src/datafog/models.py`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b2/src/datafog.egg-info/PKG-INFO` & `datafog-3.0.0b3/src/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b2 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b3 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.0.0b2/tests/test_datafog.py` & `datafog-3.0.0b3/tests/test_datafog.py`

 * *Files identical despite different names*

