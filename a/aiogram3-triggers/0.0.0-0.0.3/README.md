# Comparing `tmp/aiogram3_triggers-0.0.0.tar.gz` & `tmp/aiogram3_triggers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_triggers-0.0.0.tar", last modified: Tue Apr 23 10:13:25 2024, max compression
+gzip compressed data, was "aiogram3_triggers-0.0.3.tar", last modified: Tue Apr 23 13:24:50 2024, max compression
```

## Comparing `aiogram3_triggers-0.0.0.tar` & `aiogram3_triggers-0.0.3.tar`

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
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:24:50.202088 aiogram3_triggers-0.0.3/
+-rw-r--r--   0 dev        (501) staff       (20)    11357 2024-04-23 05:27:36.000000 aiogram3_triggers-0.0.3/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)      415 2024-04-23 13:24:50.202024 aiogram3_triggers-0.0.3/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)       39 2024-04-23 13:17:03.000000 aiogram3_triggers-0.0.3/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      103 2024-04-23 13:18:04.000000 aiogram3_triggers-0.0.3/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      507 2024-04-23 13:24:50.202349 aiogram3_triggers-0.0.3/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:24:50.200151 aiogram3_triggers-0.0.3/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:24:50.201179 aiogram3_triggers-0.0.3/src/aiogram3_triggers/
+-rw-r--r--   0 dev        (501) staff       (20)      260 2024-04-23 13:24:33.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)     8175 2024-04-23 13:23:03.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers/triggers.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-23 13:24:50.201830 aiogram3_triggers-0.0.3/src/aiogram3_triggers.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      415 2024-04-23 13:24:50.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      290 2024-04-23 13:24:50.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-23 13:24:50.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)       18 2024-04-23 13:24:50.000000 aiogram3_triggers-0.0.3/src/aiogram3_triggers.egg-info/top_level.txt
```

### Comparing `aiogram3_triggers-0.0.0/LICENSE` & `aiogram3_triggers-0.0.3/LICENSE`

 * *Files identical despite different names*

