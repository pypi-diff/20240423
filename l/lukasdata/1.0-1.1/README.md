# Comparing `tmp/lukasdata-1.0.tar.gz` & `tmp/lukasdata-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.0.tar", last modified: Sat Apr 20 07:35:40 2024, max compression
+gzip compressed data, was "lukasdata-1.1.tar", last modified: Tue Apr 23 10:52:57 2024, max compression
```

## Comparing `lukasdata-1.0.tar` & `lukasdata-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 07:35:40.336440 lukasdata-1.0/
--rw-rw-rw-   0        0        0      191 2024-04-20 07:35:40.332437 lukasdata-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-20 07:35:40.332437 lukasdata-1.0/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      191 2024-04-20 07:35:39.000000 lukasdata-1.0/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-20 07:35:40.000000 lukasdata-1.0/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:35:39.000000 lukasdata-1.0/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-20 07:35:39.000000 lukasdata-1.0/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:35:39.000000 lukasdata-1.0/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 07:35:40.336440 lukasdata-1.0/setup.cfg
--rw-rw-rw-   0        0        0      213 2024-04-20 07:34:38.000000 lukasdata-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:52:57.807134 lukasdata-1.1/
+-rw-rw-rw-   0        0        0      126 2024-04-23 10:52:57.805135 lukasdata-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 10:52:57.803134 lukasdata-1.1/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:52:57.807134 lukasdata-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      190 2024-04-23 10:47:02.000000 lukasdata-1.1/setup.py
```

