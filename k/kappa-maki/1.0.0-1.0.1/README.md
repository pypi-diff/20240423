# Comparing `tmp/kappa_maki-1.0.0.tar.gz` & `tmp/kappa_maki-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappa_maki-1.0.0.tar", max compression
+gzip compressed data, was "kappa_maki-1.0.1.tar", max compression
```

## Comparing `kappa_maki-1.0.0.tar` & `kappa_maki-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1075 2024-04-23 17:47:08.560267 kappa_maki-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      510 2024-04-23 17:47:23.727839 kappa_maki-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 17:47:08.560757 kappa_maki-1.0.0/src/kappa_maki/__init__.py
--rw-r--r--   0        0        0     8663 2024-04-23 17:47:08.560929 kappa_maki-1.0.0/src/kappa_maki/kappa_maki_formatter.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 kappa_maki-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-23 20:10:38.158793 kappa_maki-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1307 2024-04-23 20:10:38.158891 kappa_maki-1.0.1/README.md
+-rw-r--r--   0        0        0      594 2024-04-23 20:10:47.131897 kappa_maki-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 20:10:38.159244 kappa_maki-1.0.1/src/kappa_maki/__init__.py
+-rw-r--r--   0        0        0     8663 2024-04-23 20:10:38.159412 kappa_maki-1.0.1/src/kappa_maki/kappa_maki_formatter.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 kappa_maki-1.0.1/PKG-INFO
```

### Comparing `kappa_maki-1.0.0/LICENSE.txt` & `kappa_maki-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kappa_maki-1.0.0/src/kappa_maki/kappa_maki_formatter.py` & `kappa_maki-1.0.1/src/kappa_maki/kappa_maki_formatter.py`

 * *Files identical despite different names*

