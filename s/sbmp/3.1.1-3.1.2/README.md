# Comparing `tmp/sbmp-3.1.1.tar.gz` & `tmp/sbmp-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmp-3.1.1.tar", last modified: Mon Apr 22 17:00:35 2024, max compression
+gzip compressed data, was "sbmp-3.1.2.tar", last modified: Mon Apr 22 17:02:16 2024, max compression
```

## Comparing `sbmp-3.1.1.tar` & `sbmp-3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:00:35.194282 sbmp-3.1.1/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-3.1.1/LICENSE
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      456 2024-04-22 17:00:35.194019 sbmp-3.1.1/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-3.1.1/README.txt
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:00:35.192913 sbmp-3.1.1/sbmp/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       18 2024-01-08 11:36:04.000000 sbmp-3.1.1/sbmp/__init__.py
--rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-3.1.1/sbmp/iss.py
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:00:35.193840 sbmp-3.1.1/sbmp.egg-info/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      456 2024-04-22 17:00:35.000000 sbmp-3.1.1/sbmp.egg-info/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      168 2024-04-22 17:00:35.000000 sbmp-3.1.1/sbmp.egg-info/SOURCES.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-22 17:00:35.000000 sbmp-3.1.1/sbmp.egg-info/dependency_links.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-22 17:00:35.000000 sbmp-3.1.1/sbmp.egg-info/top_level.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-22 17:00:35.194334 sbmp-3.1.1/setup.cfg
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      629 2024-04-22 17:00:30.000000 sbmp-3.1.1/setup.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.726237 sbmp-3.1.2/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-3.1.2/LICENSE
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-22 17:02:16.725955 sbmp-3.1.2/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-3.1.2/README.txt
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.724910 sbmp-3.1.2/sbmp/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       18 2024-01-08 11:36:04.000000 sbmp-3.1.2/sbmp/__init__.py
+-rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-3.1.2/sbmp/iss.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.725702 sbmp-3.1.2/sbmp.egg-info/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      168 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/top_level.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-22 17:02:16.726285 sbmp-3.1.2/setup.cfg
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-22 17:02:13.000000 sbmp-3.1.2/setup.py
```

### Comparing `sbmp-3.1.1/LICENSE` & `sbmp-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmp-3.1.1/sbmp/iss.py` & `sbmp-3.1.2/sbmp/iss.py`

 * *Files identical despite different names*

