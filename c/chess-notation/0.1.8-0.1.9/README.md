# Comparing `tmp/chess_notation-0.1.8.tar.gz` & `tmp/chess_notation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_notation-0.1.8.tar", last modified: Tue Apr 23 08:41:43 2024, max compression
+gzip compressed data, was "chess_notation-0.1.9.tar", last modified: Tue Apr 23 08:43:57 2024, max compression
```

## Comparing `chess_notation-0.1.8.tar` & `chess_notation-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess_notation-0.1.8/MANIFEST.in
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:41:43.668373 chess_notation-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess_notation-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-23 08:41:40.000000 chess_notation-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:41:43.668373 chess_notation-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/chess_notation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-23 08:41:04.000000 chess_notation-0.1.8/src/chess_notation/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-23 08:41:35.000000 chess_notation-0.1.8/src/chess_notation/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/chess_notation/language/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess_notation-0.1.8/src/chess_notation/language/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess_notation-0.1.8/src/chess_notation/language/language.py
--rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess_notation-0.1.8/src/chess_notation/language/translations.json
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation/represent/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess_notation-0.1.8/src/chess_notation/represent/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1873 2024-04-16 06:53:54.000000 chess_notation-0.1.8/src/chess_notation/represent/represent.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation/styles/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess_notation-0.1.8/src/chess_notation/styles/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1329 2024-04-04 08:49:59.000000 chess_notation-0.1.8/src/chess_notation/styles/apply.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess_notation-0.1.8/src/chess_notation/styles/classify.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2364 2024-04-04 08:49:34.000000 chess_notation-0.1.8/src/chess_notation/styles/map.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess_notation-0.1.8/src/chess_notation/styles/styles.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      697 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess_notation-0.1.9/MANIFEST.in
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:43:57.114516 chess_notation-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess_notation-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-23 08:43:54.000000 chess_notation-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:43:57.114516 chess_notation-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.104516 chess_notation-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/src/chess_notation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-23 08:41:04.000000 chess_notation-0.1.9/src/chess_notation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      362 2024-04-23 08:43:47.000000 chess_notation-0.1.9/src/chess_notation/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/src/chess_notation/language/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess_notation-0.1.9/src/chess_notation/language/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess_notation-0.1.9/src/chess_notation/language/language.py
+-rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess_notation-0.1.9/src/chess_notation/language/translations.json
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/src/chess_notation/represent/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess_notation-0.1.9/src/chess_notation/represent/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1873 2024-04-16 06:53:54.000000 chess_notation-0.1.9/src/chess_notation/represent/represent.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/src/chess_notation/styles/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess_notation-0.1.9/src/chess_notation/styles/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1329 2024-04-04 08:49:59.000000 chess_notation-0.1.9/src/chess_notation/styles/apply.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess_notation-0.1.9/src/chess_notation/styles/classify.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2364 2024-04-04 08:49:34.000000 chess_notation-0.1.9/src/chess_notation/styles/map.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess_notation-0.1.9/src/chess_notation/styles/styles.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:43:57.114516 chess_notation-0.1.9/src/chess_notation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:43:57.000000 chess_notation-0.1.9/src/chess_notation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      697 2024-04-23 08:43:57.000000 chess_notation-0.1.9/src/chess_notation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:43:57.000000 chess_notation-0.1.9/src/chess_notation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-23 08:43:57.000000 chess_notation-0.1.9/src/chess_notation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-23 08:43:57.000000 chess_notation-0.1.9/src/chess_notation.egg-info/top_level.txt
```

### Comparing `chess_notation-0.1.8/src/chess_notation/language/language.py` & `chess_notation-0.1.9/src/chess_notation/language/language.py`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation/language/translations.json` & `chess_notation-0.1.9/src/chess_notation/language/translations.json`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation/represent/represent.py` & `chess_notation-0.1.9/src/chess_notation/represent/represent.py`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation/styles/apply.py` & `chess_notation-0.1.9/src/chess_notation/styles/apply.py`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation/styles/classify.py` & `chess_notation-0.1.9/src/chess_notation/styles/classify.py`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation/styles/map.py` & `chess_notation-0.1.9/src/chess_notation/styles/map.py`

 * *Files identical despite different names*

### Comparing `chess_notation-0.1.8/src/chess_notation.egg-info/SOURCES.txt` & `chess_notation-0.1.9/src/chess_notation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

