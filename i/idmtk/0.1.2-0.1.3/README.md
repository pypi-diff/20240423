# Comparing `tmp/idmtk-0.1.2.tar.gz` & `tmp/idmtk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idmtk-0.1.2.tar", max compression
+gzip compressed data, was "idmtk-0.1.3.tar", max compression
```

## Comparing `idmtk-0.1.2.tar` & `idmtk-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650796 idmtk-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650757 idmtk-0.1.2/idmtk/__init__.py
--rw-r--r--   0        0        0      805 2024-04-19 03:06:45.219869 idmtk-0.1.2/idmtk/auth.py
--rw-r--r--   0        0        0      320 2024-04-19 02:50:55.137937 idmtk-0.1.2/idmtk/models.py
--rw-r--r--   0        0        0      313 2024-04-19 03:08:18.362609 idmtk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 idmtk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650796 idmtk-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650757 idmtk-0.1.3/idmtk/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-19 03:11:32.442573 idmtk-0.1.3/idmtk/auth.py
+-rw-r--r--   0        0        0      320 2024-04-19 03:14:44.151189 idmtk-0.1.3/idmtk/models.py
+-rw-r--r--   0        0        0      312 2024-04-23 03:45:40.423009 idmtk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 idmtk-0.1.3/PKG-INFO
```

### Comparing `idmtk-0.1.2/idmtk/auth.py` & `idmtk-0.1.3/idmtk/auth.py`

 * *Files identical despite different names*

