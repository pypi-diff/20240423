# Comparing `tmp/lukasdata-1.1.tar.gz` & `tmp/lukasdata-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.1.tar", last modified: Tue Apr 23 10:52:57 2024, max compression
+gzip compressed data, was "lukasdata-1.2.tar", last modified: Tue Apr 23 21:51:14 2024, max compression
```

## Comparing `lukasdata-1.1.tar` & `lukasdata-1.2.tar`

### file list

```diff
@@ -1,10 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:52:57.807134 lukasdata-1.1/
--rw-rw-rw-   0        0        0      126 2024-04-23 10:52:57.805135 lukasdata-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 10:52:57.803134 lukasdata-1.1/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:52:57.000000 lukasdata-1.1/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 10:52:57.807134 lukasdata-1.1/setup.cfg
--rw-rw-rw-   0        0        0      190 2024-04-23 10:47:02.000000 lukasdata-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:51:14.624640 lukasdata-1.2/
+-rw-rw-rw-   0        0        0      126 2024-04-23 21:51:14.622642 lukasdata-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 21:51:14.601312 lukasdata-1.2/lukasdata/
+-rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/change_directory.py
+-rw-rw-rw-   0        0        0      200 2024-04-23 12:30:13.000000 lukasdata-1.2/lukasdata/concat_dfs.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/count_nans.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/create_mask.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/dict_to_json.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/get_number_columns.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/json_to_dict.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/list_to_string.py
+-rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/plot_metric_history.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2/lukasdata/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:51:14.620643 lukasdata-1.2/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-23 21:51:14.000000 lukasdata-1.2/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2024-04-23 21:51:14.000000 lukasdata-1.2/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 21:51:14.000000 lukasdata-1.2/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 21:51:14.000000 lukasdata-1.2/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-23 21:51:14.000000 lukasdata-1.2/lukasdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 21:51:14.625640 lukasdata-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      190 2024-04-23 21:50:15.000000 lukasdata-1.2/setup.py
```

