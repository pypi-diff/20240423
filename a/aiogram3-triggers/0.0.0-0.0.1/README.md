# Comparing `tmp/aiogram3_triggers-0.0.0.tar.gz` & `tmp/aiogram3_triggers-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_triggers-0.0.0.tar", last modified: Tue Apr 23 10:13:25 2024, max compression
+gzip compressed data, was "aiogram3_triggers-0.0.1.tar", last modified: Tue Apr 23 13:00:55 2024, max compression
```

## Comparing `aiogram3_triggers-0.0.0.tar` & `aiogram3_triggers-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 10:13:25.955685 aiogram3_triggers-0.0.0/
--rw-r--r--   0 dev        (501) staff       (20)    11357 2024-04-23 05:27:36.000000 aiogram3_triggers-0.0.0/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)     1239 2024-04-23 10:13:25.955618 aiogram3_triggers-0.0.0/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      863 2024-04-23 10:05:57.000000 aiogram3_triggers-0.0.0/README.md
--rw-r--r--   0 dev        (501) staff       (20)      103 2024-04-23 10:06:27.000000 aiogram3_triggers-0.0.0/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      506 2024-04-23 10:13:25.955947 aiogram3_triggers-0.0.0/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 10:13:25.952900 aiogram3_triggers-0.0.0/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 10:13:25.954269 aiogram3_triggers-0.0.0/src/aiogram3_triggers/
--rw-r--r--   0 dev        (501) staff       (20)      260 2024-04-23 10:02:31.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)     3755 2024-04-23 10:02:16.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers/triggers.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 10:13:25.955411 aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)     1239 2024-04-23 10:13:25.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      290 2024-04-23 10:13:25.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-23 10:13:25.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)       18 2024-04-23 10:13:25.000000 aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:00:55.273849 aiogram3_triggers-0.0.1/
+-rw-r--r--   0 dev        (501) staff       (20)    11357 2024-04-23 05:27:36.000000 aiogram3_triggers-0.0.1/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)     1239 2024-04-23 13:00:55.273748 aiogram3_triggers-0.0.1/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      863 2024-04-23 10:05:57.000000 aiogram3_triggers-0.0.1/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      103 2024-04-23 10:06:27.000000 aiogram3_triggers-0.0.1/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      506 2024-04-23 13:00:55.274209 aiogram3_triggers-0.0.1/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:00:55.271413 aiogram3_triggers-0.0.1/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:00:55.272685 aiogram3_triggers-0.0.1/src/aiogram3_triggers/
+-rw-r--r--   0 dev        (501) staff       (20)      260 2024-04-23 12:23:08.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)     8154 2024-04-23 12:59:27.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers/triggers.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:00:55.273495 aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)     1239 2024-04-23 13:00:55.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      290 2024-04-23 13:00:55.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-23 13:00:55.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)       18 2024-04-23 13:00:55.000000 aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/top_level.txt
```

### Comparing `aiogram3_triggers-0.0.0/LICENSE` & `aiogram3_triggers-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_triggers-0.0.0/PKG-INFO` & `aiogram3_triggers-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-triggers
-Version: 0.0.0
+Version: 0.0.1
 Summary: Aiogra3 Triggers
 Home-page: https://github.com/zcxw-code/aiogram3-triggers
 Author: Zcxw
 Author-email: zcxw.code@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `aiogram3_triggers-0.0.0/README.md` & `aiogram3_triggers-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_triggers-0.0.0/src/aiogram3_triggers.egg-info/PKG-INFO` & `aiogram3_triggers-0.0.1/src/aiogram3_triggers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-triggers
-Version: 0.0.0
+Version: 0.0.1
 Summary: Aiogra3 Triggers
 Home-page: https://github.com/zcxw-code/aiogram3-triggers
 Author: Zcxw
 Author-email: zcxw.code@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

