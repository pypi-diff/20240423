# Comparing `tmp/nestipy_ioc-0.1.2.tar.gz` & `tmp/nestipy_ioc-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_ioc-0.1.2.tar", max compression
+gzip compressed data, was "nestipy_ioc-0.1.20.tar", max compression
```

## Comparing `nestipy_ioc-0.1.2.tar` & `nestipy_ioc-0.1.20.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.2/README.md
--rw-r--r--   0        0        0      373 2024-04-23 15:32:06.434233 nestipy_ioc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      589 2024-04-23 15:31:43.394306 nestipy_ioc-0.1.2/src/nestipy_ioc/__init__.py
--rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.2/src/nestipy_ioc/annotation.py
--rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.2/src/nestipy_ioc/container.py
--rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.2/src/nestipy_ioc/context_container.py
--rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.2/src/nestipy_ioc/dependency.py
--rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.2/src/nestipy_ioc/meta.py
--rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.2/src/nestipy_ioc/provider.py
--rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.2/src/nestipy_ioc/utils.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.20/README.md
+-rw-r--r--   0        0        0      374 2024-04-23 15:39:11.296897 nestipy_ioc-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0      589 2024-04-23 15:31:43.394306 nestipy_ioc-0.1.20/src/nestipy_ioc/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.20/src/nestipy_ioc/annotation.py
+-rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.20/src/nestipy_ioc/container.py
+-rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.20/src/nestipy_ioc/context_container.py
+-rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.20/src/nestipy_ioc/dependency.py
+-rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.20/src/nestipy_ioc/meta.py
+-rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.20/src/nestipy_ioc/provider.py
+-rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.20/src/nestipy_ioc/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.20/PKG-INFO
```

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/__init__.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/container.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/context_container.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/dependency.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/meta.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.2/src/nestipy_ioc/provider.py` & `nestipy_ioc-0.1.20/src/nestipy_ioc/provider.py`

 * *Files identical despite different names*

