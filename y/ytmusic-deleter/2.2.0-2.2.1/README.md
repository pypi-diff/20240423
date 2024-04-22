# Comparing `tmp/ytmusic_deleter-2.2.0.tar.gz` & `tmp/ytmusic_deleter-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.2.0.tar", last modified: Mon Apr 22 22:27:15 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.2.1.tar", last modified: Mon Apr 22 23:08:19 2024, max compression
```

## Comparing `ytmusic_deleter-2.2.0.tar` & `ytmusic_deleter-2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-22 22:26:59.655954 ytmusic_deleter-2.2.0/LICENSE
--rw-r--r--   0        0        0     1493 2024-04-22 22:27:15.544189 ytmusic_deleter-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5030 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1304 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/tests/resources/test.example.cfg
--rw-r--r--   0        0        0     2869 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     5475 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/README.md
--rw-r--r--   0        0        0       22 2024-04-22 22:27:15.540189 ytmusic_deleter-2.2.0/ytmusic_deleter/_version.py
--rw-r--r--   0        0        0     1270 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/auth.py
--rw-r--r--   0        0        0    17213 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/cli.py
--rw-r--r--   0        0        0      168 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/constants.py
--rw-r--r--   0        0        0      319 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/progress.py
--rw-r--r--   0        0        0     9521 2024-04-22 22:26:59.659954 ytmusic_deleter-2.2.0/ytmusic_deleter/uploads.py
--rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-22 23:08:02.008007 ytmusic_deleter-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1493 2024-04-22 23:08:19.852197 ytmusic_deleter-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5030 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1304 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/tests/resources/test.example.cfg
+-rw-r--r--   0        0        0     2869 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/tests/test_cli.py
+-rw-r--r--   0        0        0     5475 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/README.md
+-rw-r--r--   0        0        0       22 2024-04-22 23:08:19.852197 ytmusic_deleter-2.2.1/ytmusic_deleter/_version.py
+-rw-r--r--   0        0        0     1270 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/auth.py
+-rw-r--r--   0        0        0    17213 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/cli.py
+-rw-r--r--   0        0        0      168 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/constants.py
+-rw-r--r--   0        0        0      319 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/progress.py
+-rw-r--r--   0        0        0     9521 2024-04-22 23:08:02.016007 ytmusic_deleter-2.2.1/ytmusic_deleter/uploads.py
+-rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.2.1/PKG-INFO
```

### Comparing `ytmusic_deleter-2.2.0/LICENSE` & `ytmusic_deleter-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/pyproject.toml` & `ytmusic_deleter-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "click>=8.1.7",
     "enlighten>=1.12.4",
     "thefuzz>=0.22.1",
     "ytmusicapi>=1.6.0",
 ]
 requires-python = "<3.13,>=3.8.1"
 readme = "ytmusic_deleter/README.md"
-version = "2.2.0"
+version = "2.2.1"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.scripts]
 ytmusic-deleter = "ytmusic_deleter.cli:cli"
```

### Comparing `ytmusic_deleter-2.2.0/tests/conftest.py` & `ytmusic_deleter-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/tests/resources/test.example.cfg` & `ytmusic_deleter-2.2.1/tests/resources/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/tests/test_cli.py` & `ytmusic_deleter-2.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/ytmusic_deleter/README.md` & `ytmusic_deleter-2.2.1/ytmusic_deleter/README.md`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/ytmusic_deleter/auth.py` & `ytmusic_deleter-2.2.1/ytmusic_deleter/auth.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/ytmusic_deleter/cli.py` & `ytmusic_deleter-2.2.1/ytmusic_deleter/cli.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/ytmusic_deleter/uploads.py` & `ytmusic_deleter-2.2.1/ytmusic_deleter/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.0/PKG-INFO` & `ytmusic_deleter-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusic-deleter
-Version: 2.2.0
+Version: 2.2.1
 Summary: Easily delete your YouTube Music library
 Author-Email: apastel <alex.r.pastel@gmail.com>
 License: GPL-3.0
 Requires-Python: <3.13,>=3.8.1
 Requires-Dist: click>=8.1.7
 Requires-Dist: enlighten>=1.12.4
 Requires-Dist: thefuzz>=0.22.1
```

