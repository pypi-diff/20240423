# Comparing `tmp/lib_repo_tool-2.0.6.tar.gz` & `tmp/lib_repo_tool-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_repo_tool-2.0.6.tar", last modified: Mon Sep 25 08:05:01 2023, max compression
+gzip compressed data, was "lib_repo_tool-2.0.7.tar", last modified: Tue Apr 23 04:37:48 2024, max compression
```

## Comparing `lib_repo_tool-2.0.6.tar` & `lib_repo_tool-2.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-09-25 08:05:01.704815 lib_repo_tool-2.0.6/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-09-25 08:05:01.704492 lib_repo_tool-2.0.6/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.6/README.md
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-09-25 08:05:01.702358 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      327 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/SOURCES.txt
--rw-r--r--   0 Andy       (501) staff       (20)        1 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/dependency_links.txt
--rw-r--r--   0 Andy       (501) staff       (20)       76 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/entry_points.txt
--rw-r--r--   0 Andy       (501) staff       (20)       36 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/requires.txt
--rw-r--r--   0 Andy       (501) staff       (20)       10 2023-09-25 08:05:01.000000 lib_repo_tool-2.0.6/lib_repo_tool.egg-info/top_level.txt
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-09-25 08:05:01.703941 lib_repo_tool-2.0.6/repo_tool/
--rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.6/repo_tool/__init__.py
--rw-r--r--   0 Andy       (501) staff       (20)     5815 2023-09-25 08:01:52.000000 lib_repo_tool-2.0.6/repo_tool/common.py
--rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.6/repo_tool/lib_get.py
--rw-r--r--   0 Andy       (501) staff       (20)    17098 2023-09-25 07:59:40.000000 lib_repo_tool-2.0.6/repo_tool/lib_repo.py
--rw-r--r--   0 Andy       (501) staff       (20)       38 2023-09-25 08:05:01.704935 lib_repo_tool-2.0.6/setup.cfg
--rw-r--r--   0 Andy       (501) staff       (20)      473 2023-09-25 08:04:30.000000 lib_repo_tool-2.0.6/setup.py
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2024-04-23 04:37:48.128996 lib_repo_tool-2.0.7/
+-rw-r--r--   0 Andy       (501) staff       (20)      227 2024-04-23 04:37:48.128771 lib_repo_tool-2.0.7/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.7/README.md
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2024-04-23 04:37:48.125259 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/
+-rw-r--r--   0 Andy       (501) staff       (20)      227 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      327 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 Andy       (501) staff       (20)        1 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       77 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/entry_points.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       36 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/requires.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       10 2024-04-23 04:37:48.000000 lib_repo_tool-2.0.7/lib_repo_tool.egg-info/top_level.txt
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2024-04-23 04:37:48.127728 lib_repo_tool-2.0.7/repo_tool/
+-rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.7/repo_tool/__init__.py
+-rw-r--r--   0 Andy       (501) staff       (20)     5817 2024-04-23 02:59:02.000000 lib_repo_tool-2.0.7/repo_tool/common.py
+-rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.7/repo_tool/lib_get.py
+-rw-r--r--   0 Andy       (501) staff       (20)    17098 2023-09-25 07:59:40.000000 lib_repo_tool-2.0.7/repo_tool/lib_repo.py
+-rw-r--r--   0 Andy       (501) staff       (20)       38 2024-04-23 04:37:48.129090 lib_repo_tool-2.0.7/setup.cfg
+-rw-r--r--   0 Andy       (501) staff       (20)      473 2024-04-23 04:37:30.000000 lib_repo_tool-2.0.7/setup.py
```

### Comparing `lib_repo_tool-2.0.6/README.md` & `lib_repo_tool-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.6/repo_tool/common.py` & `lib_repo_tool-2.0.7/repo_tool/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 # def download_file(file_key, to_path):
     # get_bucket().get_object_to_file(file_key, to_path)
 
 def get_download_url(file_key):
     cdn_key = CDN_URL_SIGN_KEY
     download_url = ''
     if cdn_key:
-        raw_url = parse.urljoin('http://oss.lib-repo.dev.arcsiteapp.cn', file_key)
+        raw_url = parse.urljoin('http://oss.lib-repo.dev.shexiangyun.com', file_key)
         exp = int(time.time()) + 1 * 3600
         download_url = a_auth(raw_url, cdn_key, exp)
     else:
         download_url: str = get_bucket().sign_url('GET', file_key, 60 * 30) 
 
     return download_url
```

### Comparing `lib_repo_tool-2.0.6/repo_tool/lib_get.py` & `lib_repo_tool-2.0.7/repo_tool/lib_get.py`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.6/repo_tool/lib_repo.py` & `lib_repo_tool-2.0.7/repo_tool/lib_repo.py`

 * *Files identical despite different names*

