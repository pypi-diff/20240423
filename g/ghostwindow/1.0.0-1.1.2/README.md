# Comparing `tmp/ghostwindow-1.0.0.tar.gz` & `tmp/ghostwindow-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostwindow-1.0.0.tar", last modified: Wed Feb 21 00:59:06 2024, max compression
+gzip compressed data, was "ghostwindow-1.1.2.tar", last modified: Tue Apr 23 03:45:56 2024, max compression
```

## Comparing `ghostwindow-1.0.0.tar` & `ghostwindow-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 00:59:06.035817 ghostwindow-1.0.0/
--rw-rw-rw-   0        0        0      512 2024-02-21 00:59:06.035817 ghostwindow-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-19 02:24:52.000000 ghostwindow-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2024-02-19 02:31:39.000000 ghostwindow-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      676 2024-02-21 00:59:06.036815 ghostwindow-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-21 00:59:06.026514 ghostwindow-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-21 00:59:06.028844 ghostwindow-1.0.0/src/ghostwindow/
--rw-rw-rw-   0        0        0     5588 2024-02-20 05:20:48.000000 ghostwindow-1.0.0/src/ghostwindow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-21 00:59:06.034821 ghostwindow-1.0.0/src/ghostwindow.egg-info/
--rw-rw-rw-   0        0        0      512 2024-02-21 00:59:06.000000 ghostwindow-1.0.0/src/ghostwindow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-02-21 00:59:06.000000 ghostwindow-1.0.0/src/ghostwindow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 00:59:06.000000 ghostwindow-1.0.0/src/ghostwindow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-21 00:59:06.000000 ghostwindow-1.0.0/src/ghostwindow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 03:45:56.689598 ghostwindow-1.1.2/
+-rw-rw-rw-   0        0        0     3172 2024-04-23 03:45:56.688598 ghostwindow-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2533 2024-04-23 03:38:44.000000 ghostwindow-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 03:45:56.688598 ghostwindow-1.1.2/ghostwindow.egg-info/
+-rw-rw-rw-   0        0        0     3172 2024-04-23 03:45:56.000000 ghostwindow-1.1.2/ghostwindow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-04-23 03:45:56.000000 ghostwindow-1.1.2/ghostwindow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:45:56.000000 ghostwindow-1.1.2/ghostwindow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:45:56.000000 ghostwindow-1.1.2/ghostwindow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2024-04-02 01:27:43.000000 ghostwindow-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 03:45:56.689598 ghostwindow-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      914 2024-04-23 03:45:12.000000 ghostwindow-1.1.2/setup.py
```

