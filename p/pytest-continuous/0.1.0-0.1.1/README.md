# Comparing `tmp/pytest-continuous-0.1.0.tar.gz` & `tmp/pytest-continuous-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-continuous-0.1.0.tar", last modified: Tue Apr 23 06:49:36 2024, max compression
+gzip compressed data, was "pytest-continuous-0.1.1.tar", last modified: Tue Apr 23 08:06:11 2024, max compression
```

## Comparing `pytest-continuous-0.1.0.tar` & `pytest-continuous-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 06:49:36.213778 pytest-continuous-0.1.0/
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      293 2024-04-23 06:49:36.209776 pytest-continuous-0.1.0/PKG-INFO
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      221 2024-04-23 06:48:36.000000 pytest-continuous-0.1.0/README.md
-drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 06:49:36.209776 pytest-continuous-0.1.0/pytest_continuous/
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 06:09:04.000000 pytest-continuous-0.1.0/pytest_continuous/__init__.py
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)     1072 2024-04-23 06:45:06.000000 pytest-continuous-0.1.0/pytest_continuous/plugin.py
-drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 06:49:36.209776 pytest-continuous-0.1.0/pytest_continuous.egg-info/
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      293 2024-04-23 06:49:36.000000 pytest-continuous-0.1.0/pytest_continuous.egg-info/PKG-INFO
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      284 2024-04-23 06:49:36.000000 pytest-continuous-0.1.0/pytest_continuous.egg-info/SOURCES.txt
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)        1 2024-04-23 06:49:36.000000 pytest-continuous-0.1.0/pytest_continuous.egg-info/dependency_links.txt
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       49 2024-04-23 06:49:36.000000 pytest-continuous-0.1.0/pytest_continuous.egg-info/entry_points.txt
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       18 2024-04-23 06:49:36.000000 pytest-continuous-0.1.0/pytest_continuous.egg-info/top_level.txt
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       38 2024-04-23 06:49:36.213778 pytest-continuous-0.1.0/setup.cfg
--rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      508 2024-04-23 06:19:35.000000 pytest-continuous-0.1.0/setup.py
+drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 08:06:11.683034 pytest-continuous-0.1.1/
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      293 2024-04-23 08:06:11.683034 pytest-continuous-0.1.1/PKG-INFO
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      382 2024-04-23 08:05:31.000000 pytest-continuous-0.1.1/README.md
+drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 08:06:11.683034 pytest-continuous-0.1.1/pytest_continuous/
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 06:09:04.000000 pytest-continuous-0.1.1/pytest_continuous/__init__.py
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)     1072 2024-04-23 06:45:06.000000 pytest-continuous-0.1.1/pytest_continuous/plugin.py
+drwxrwxr-x   0 zhongsufan  (1000) zhongsufan  (1000)        0 2024-04-23 08:06:11.683034 pytest-continuous-0.1.1/pytest_continuous.egg-info/
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      293 2024-04-23 08:06:11.000000 pytest-continuous-0.1.1/pytest_continuous.egg-info/PKG-INFO
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      284 2024-04-23 08:06:11.000000 pytest-continuous-0.1.1/pytest_continuous.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)        1 2024-04-23 08:06:11.000000 pytest-continuous-0.1.1/pytest_continuous.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       49 2024-04-23 08:06:11.000000 pytest-continuous-0.1.1/pytest_continuous.egg-info/entry_points.txt
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       18 2024-04-23 08:06:11.000000 pytest-continuous-0.1.1/pytest_continuous.egg-info/top_level.txt
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)       38 2024-04-23 08:06:11.683034 pytest-continuous-0.1.1/setup.cfg
+-rw-rw-r--   0 zhongsufan  (1000) zhongsufan  (1000)      508 2024-04-23 08:05:44.000000 pytest-continuous-0.1.1/setup.py
```

### Comparing `pytest-continuous-0.1.0/pytest_continuous/plugin.py` & `pytest-continuous-0.1.1/pytest_continuous/plugin.py`

 * *Files identical despite different names*

