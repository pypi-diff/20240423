# Comparing `tmp/python_shinkansen-0.7.3.tar.gz` & `tmp/python_shinkansen-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_shinkansen-0.7.3.tar", max compression
+gzip compressed data, was "python_shinkansen-0.7.4.tar", max compression
```

## Comparing `python_shinkansen-0.7.3.tar` & `python_shinkansen-0.7.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      519 2023-11-29 11:28:57.656009 python_shinkansen-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-11-29 11:29:02.993335 python_shinkansen-0.7.3/shinkansen/__init__.py
--rw-r--r--   0        0        0     3904 2022-10-25 19:58:12.923345 python_shinkansen-0.7.3/shinkansen/common.py
--rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.7.3/shinkansen/jws.py
--rw-r--r--   0        0        0    12652 2023-06-05 05:39:29.564730 python_shinkansen-0.7.3/shinkansen/payins.py
--rw-r--r--   0        0        0    10245 2023-11-17 14:09:18.988431 python_shinkansen-0.7.3/shinkansen/payouts.py
--rw-r--r--   0        0        0     7818 2023-06-05 04:17:49.043149 python_shinkansen-0.7.3/shinkansen/responses.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 python_shinkansen-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      520 2024-04-23 13:49:03.689560 python_shinkansen-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-23 13:49:12.479564 python_shinkansen-0.7.4/shinkansen/__init__.py
+-rw-r--r--   0        0        0     8440 2024-04-23 13:20:10.410585 python_shinkansen-0.7.4/shinkansen/common.py
+-rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.7.4/shinkansen/jws.py
+-rw-r--r--   0        0        0    12652 2023-06-05 05:39:29.564730 python_shinkansen-0.7.4/shinkansen/payins.py
+-rw-r--r--   0        0        0    10245 2023-11-17 14:09:18.988431 python_shinkansen-0.7.4/shinkansen/payouts.py
+-rw-r--r--   0        0        0     7818 2023-06-05 04:17:49.043149 python_shinkansen-0.7.4/shinkansen/responses.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 python_shinkansen-0.7.4/PKG-INFO
```

### Comparing `python_shinkansen-0.7.3/shinkansen/jws.py` & `python_shinkansen-0.7.4/shinkansen/jws.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.3/shinkansen/payins.py` & `python_shinkansen-0.7.4/shinkansen/payins.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.3/shinkansen/payouts.py` & `python_shinkansen-0.7.4/shinkansen/payouts.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.3/shinkansen/responses.py` & `python_shinkansen-0.7.4/shinkansen/responses.py`

 * *Files identical despite different names*

