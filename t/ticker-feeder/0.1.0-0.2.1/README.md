# Comparing `tmp/ticker_feeder-0.1.0.tar.gz` & `tmp/ticker_feeder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticker_feeder-0.1.0.tar", last modified: Tue Apr 23 20:55:07 2024, max compression
+gzip compressed data, was "ticker_feeder-0.2.1.tar", last modified: Tue Apr 23 21:19:42 2024, max compression
```

## Comparing `ticker_feeder-0.1.0.tar` & `ticker_feeder-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:55:07.600615 ticker_feeder-0.1.0/
--rw-rw-rw-   0        0        0      489 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      353 2024-04-23 20:55:07.599613 ticker_feeder-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 20:55:07.600615 ticker_feeder-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      486 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:55:07.592089 ticker_feeder-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      160 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/tests/test_feeder.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:55:07.593089 ticker_feeder-0.1.0/ticker_feeder/
--rw-rw-rw-   0        0        0        0 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/ticker_feeder/__init__.py
--rw-rw-rw-   0        0        0       51 2024-04-23 20:55:03.000000 ticker_feeder-0.1.0/ticker_feeder/feeder.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:55:07.597615 ticker_feeder-0.1.0/ticker_feeder.egg-info/
--rw-rw-rw-   0        0        0      353 2024-04-23 20:55:07.000000 ticker_feeder-0.1.0/ticker_feeder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-23 20:55:07.000000 ticker_feeder-0.1.0/ticker_feeder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:55:07.000000 ticker_feeder-0.1.0/ticker_feeder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 20:55:07.000000 ticker_feeder-0.1.0/ticker_feeder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 21:19:42.705095 ticker_feeder-0.2.1/
+-rw-rw-rw-   0        0        0      489 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      356 2024-04-23 21:19:42.704140 ticker_feeder-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 21:19:42.705095 ticker_feeder-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-04-23 21:18:56.000000 ticker_feeder-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:19:42.695560 ticker_feeder-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/tests/test_feeder.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:19:42.696571 ticker_feeder-0.2.1/ticker_feeder/
+-rw-rw-rw-   0        0        0        0 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/ticker_feeder/__init__.py
+-rw-rw-rw-   0        0        0       51 2024-04-23 20:55:03.000000 ticker_feeder-0.2.1/ticker_feeder/feeder.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:19:42.701566 ticker_feeder-0.2.1/ticker_feeder.egg-info/
+-rw-rw-rw-   0        0        0      356 2024-04-23 21:19:42.000000 ticker_feeder-0.2.1/ticker_feeder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-23 21:19:42.000000 ticker_feeder-0.2.1/ticker_feeder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 21:19:42.000000 ticker_feeder-0.2.1/ticker_feeder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 21:19:42.000000 ticker_feeder-0.2.1/ticker_feeder.egg-info/top_level.txt
```

