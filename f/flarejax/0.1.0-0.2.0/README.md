# Comparing `tmp/flarejax-0.1.0.tar.gz` & `tmp/flarejax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarejax-0.1.0.tar", last modified: Sat Feb 17 14:21:09 2024, max compression
+gzip compressed data, was "flarejax-0.2.0.tar", last modified: Tue Apr 23 00:26:15 2024, max compression
```

## Comparing `flarejax-0.1.0.tar` & `flarejax-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-02-17 14:21:09.105903 flarejax-0.1.0/
--rw-r--r--   0 anton     (1000) anton     (1000)      420 2024-02-17 14:21:09.105903 flarejax-0.1.0/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      153 2024-02-15 13:42:33.000000 flarejax-0.1.0/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-02-17 14:21:09.105903 flarejax-0.1.0/flarejax/
--rw-r--r--   0 anton     (1000) anton     (1000)      412 2024-02-17 14:18:57.000000 flarejax-0.1.0/flarejax/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)     2237 2024-02-17 14:17:18.000000 flarejax-0.1.0/flarejax/_layers.py
--rw-r--r--   0 anton     (1000) anton     (1000)     5315 2024-02-17 14:17:14.000000 flarejax-0.1.0/flarejax/_module.py
--rw-r--r--   0 anton     (1000) anton     (1000)      801 2024-02-16 15:26:42.000000 flarejax-0.1.0/flarejax/_param.py
--rw-r--r--   0 anton     (1000) anton     (1000)      941 2024-02-15 23:48:18.000000 flarejax-0.1.0/flarejax/_pytree.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-02-17 14:21:09.105903 flarejax-0.1.0/flarejax.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)      420 2024-02-17 14:21:09.000000 flarejax-0.1.0/flarejax.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      277 2024-02-17 14:21:09.000000 flarejax-0.1.0/flarejax.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-02-17 14:21:09.000000 flarejax-0.1.0/flarejax.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       31 2024-02-17 14:21:09.000000 flarejax-0.1.0/flarejax.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-02-17 14:21:09.000000 flarejax-0.1.0/flarejax.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-02-17 14:21:09.105903 flarejax-0.1.0/setup.cfg
--rw-r--r--   0 anton     (1000) anton     (1000)      648 2024-02-14 22:39:08.000000 flarejax-0.1.0/setup.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2426 2024-04-23 00:26:15.419575 flarejax-0.2.0/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)     2159 2024-04-23 00:25:39.000000 flarejax-0.2.0/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/flarejax/
+-rw-r--r--   0 anton     (1000) anton     (1000)      720 2024-04-23 00:23:31.000000 flarejax-0.2.0/flarejax/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3459 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_config.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     4687 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_frozen.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    14093 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_module.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     7749 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_mtypes.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2872 2024-04-23 00:21:25.000000 flarejax-0.2.0/flarejax/_serial.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/flarejax.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2426 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      298 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       46 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-04-23 00:26:15.419575 flarejax-0.2.0/setup.cfg
+-rw-r--r--   0 anton     (1000) anton     (1000)      648 2024-02-14 22:39:08.000000 flarejax-0.2.0/setup.py
```

### Comparing `flarejax-0.1.0/setup.py` & `flarejax-0.2.0/setup.py`

 * *Files identical despite different names*

