# Comparing `tmp/corestart-0.1.1.tar.gz` & `tmp/CoreStart-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corestart-0.1.1.tar", last modified: Mon Apr 15 07:38:47 2024, max compression
+gzip compressed data, was "CoreStart-0.1.3.tar", last modified: Tue Apr 23 07:50:12 2024, max compression
```

## Comparing `corestart-0.1.1.tar` & `CoreStart-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-15 07:38:47.789598 corestart-0.1.1/
--rw-r--r--   0 flycode77   (501) staff       (20)       37 2024-04-15 07:13:12.000000 corestart-0.1.1/MANIFEST.in
--rw-r--r--   0 flycode77   (501) staff       (20)      127 2024-04-15 07:38:47.789402 corestart-0.1.1/PKG-INFO
--rw-r--r--   0 flycode77   (501) staff       (20)        0 2024-04-15 07:08:17.000000 corestart-0.1.1/README.md
--rw-r--r--   0 flycode77   (501) staff       (20)       38 2024-04-15 07:38:47.789637 corestart-0.1.1/setup.cfg
--rw-r--r--   0 flycode77   (501) staff       (20)      476 2024-04-15 07:38:30.000000 corestart-0.1.1/setup.py
-drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-15 07:38:47.787757 corestart-0.1.1/src/
-drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-15 07:38:47.789205 corestart-0.1.1/src/CoreStart.egg-info/
--rw-r--r--   0 flycode77   (501) staff       (20)      127 2024-04-15 07:38:47.000000 corestart-0.1.1/src/CoreStart.egg-info/PKG-INFO
--rw-r--r--   0 flycode77   (501) staff       (20)      300 2024-04-15 07:38:47.000000 corestart-0.1.1/src/CoreStart.egg-info/SOURCES.txt
--rw-r--r--   0 flycode77   (501) staff       (20)        1 2024-04-15 07:38:47.000000 corestart-0.1.1/src/CoreStart.egg-info/dependency_links.txt
--rw-r--r--   0 flycode77   (501) staff       (20)       56 2024-04-15 07:38:47.000000 corestart-0.1.1/src/CoreStart.egg-info/entry_points.txt
--rw-r--r--   0 flycode77   (501) staff       (20)       10 2024-04-15 07:38:47.000000 corestart-0.1.1/src/CoreStart.egg-info/top_level.txt
-drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-15 07:38:47.789043 corestart-0.1.1/src/corestart/
--rw-r--r--   0 flycode77   (501) staff       (20)        0 2024-04-15 07:07:53.000000 corestart-0.1.1/src/corestart/__init__.py
--rw-r--r--   0 flycode77   (501) staff       (20)      222 2024-04-15 07:12:32.000000 corestart-0.1.1/src/corestart/core_start.py
--rw-r--r--   0 flycode77   (501) staff       (20)      414 2024-04-15 07:08:35.000000 corestart-0.1.1/src/corestart/core_start.sh
+drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-23 07:50:12.448274 CoreStart-0.1.3/
+-rw-r--r--   0 flycode77   (501) staff       (20)       37 2024-04-23 07:44:22.000000 CoreStart-0.1.3/MANIFEST.in
+-rw-r--r--   0 flycode77   (501) staff       (20)      127 2024-04-23 07:50:12.448097 CoreStart-0.1.3/PKG-INFO
+-rw-r--r--   0 flycode77   (501) staff       (20)        7 2024-04-23 07:44:22.000000 CoreStart-0.1.3/README.md
+-rw-r--r--   0 flycode77   (501) staff       (20)       38 2024-04-23 07:50:12.448333 CoreStart-0.1.3/setup.cfg
+-rw-r--r--   0 flycode77   (501) staff       (20)      476 2024-04-23 07:44:22.000000 CoreStart-0.1.3/setup.py
+drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-23 07:50:12.446421 CoreStart-0.1.3/src/
+drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-23 07:50:12.447573 CoreStart-0.1.3/src/CoreStart.egg-info/
+-rw-r--r--   0 flycode77   (501) staff       (20)      127 2024-04-23 07:50:12.000000 CoreStart-0.1.3/src/CoreStart.egg-info/PKG-INFO
+-rw-r--r--   0 flycode77   (501) staff       (20)      300 2024-04-23 07:50:12.000000 CoreStart-0.1.3/src/CoreStart.egg-info/SOURCES.txt
+-rw-r--r--   0 flycode77   (501) staff       (20)        1 2024-04-23 07:50:12.000000 CoreStart-0.1.3/src/CoreStart.egg-info/dependency_links.txt
+-rw-r--r--   0 flycode77   (501) staff       (20)       56 2024-04-23 07:50:12.000000 CoreStart-0.1.3/src/CoreStart.egg-info/entry_points.txt
+-rw-r--r--   0 flycode77   (501) staff       (20)       10 2024-04-23 07:50:12.000000 CoreStart-0.1.3/src/CoreStart.egg-info/top_level.txt
+drwxr-xr-x   0 flycode77   (501) staff       (20)        0 2024-04-23 07:50:12.447931 CoreStart-0.1.3/src/corestart/
+-rw-r--r--   0 flycode77   (501) staff       (20)        0 2024-04-23 07:44:22.000000 CoreStart-0.1.3/src/corestart/__init__.py
+-rw-r--r--   0 flycode77   (501) staff       (20)      222 2024-04-23 07:44:22.000000 CoreStart-0.1.3/src/corestart/core_start.py
+-rw-r--r--   0 flycode77   (501) staff       (20)     3285 2024-04-23 07:44:22.000000 CoreStart-0.1.3/src/corestart/core_start.sh
```

