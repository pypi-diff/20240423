# Comparing `tmp/grutil-0.1.2.tar.gz` & `tmp/grutil-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grutil-0.1.2.tar", max compression
+gzip compressed data, was "grutil-0.1.4.tar", max compression
```

## Comparing `grutil-0.1.2.tar` & `grutil-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      187 2024-04-23 18:15:10.298364 grutil-0.1.2/grutil/__init__.py
--rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.1.2/grutil/afm.py
--rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.1.2/grutil/amka.py
--rw-r--r--   0        0        0     1369 2024-04-23 18:51:58.450243 grutil-0.1.2/grutil/dates.py
--rw-r--r--   0        0        0      276 2024-04-23 18:54:30.809796 grutil-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.1.2/README.md
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:13.376022 grutil-0.1.4/grutil/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.1.4/grutil/afm.py
+-rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.1.4/grutil/amka.py
+-rw-r--r--   0        0        0     4843 2024-04-23 19:46:07.559037 grutil-0.1.4/grutil/dates.py
+-rw-r--r--   0        0        0      628 2024-04-23 19:52:08.437928 grutil-0.1.4/grutil/numbers.py
+-rw-r--r--   0        0        0      383 2024-04-23 19:06:07.821075 grutil-0.1.4/grutil/text.py
+-rw-r--r--   0        0        0      276 2024-04-23 19:59:48.950982 grutil-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.1.4/README.md
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.1.4/PKG-INFO
```

### Comparing `grutil-0.1.2/grutil/amka.py` & `grutil-0.1.4/grutil/amka.py`

 * *Files identical despite different names*

