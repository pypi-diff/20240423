# Comparing `tmp/linuxsysstat-0.1.0.tar.gz` & `tmp/linuxsysstat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxsysstat-0.1.0.tar", max compression
+gzip compressed data, was "linuxsysstat-0.1.1.tar", max compression
```

## Comparing `linuxsysstat-0.1.0.tar` & `linuxsysstat-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      306 2024-04-23 19:33:14.759414 linuxsysstat-0.1.0/README.md
--rwxr-xr-x   0        0        0     1101 2024-04-23 19:21:47.321483 linuxsysstat-0.1.0/linuxsysstat.py
--rw-r--r--   0        0        0      385 2024-04-23 19:23:35.225832 linuxsysstat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 linuxsysstat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      306 2024-04-23 19:33:14.759414 linuxsysstat-0.1.1/README.md
+-rwxr-xr-x   0        0        0     1101 2024-04-23 19:21:47.321483 linuxsysstat-0.1.1/linuxsysstat.py
+-rw-r--r--   0        0        0      381 2024-04-23 20:56:34.309476 linuxsysstat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 linuxsysstat-0.1.1/PKG-INFO
```

### Comparing `linuxsysstat-0.1.0/linuxsysstat.py` & `linuxsysstat-0.1.1/linuxsysstat.py`

 * *Files identical despite different names*

### Comparing `linuxsysstat-0.1.0/PKG-INFO` & `linuxsysstat-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxsysstat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Linux System stat
 License: MIT
 Author: Bharath
 Author-email: learnit.linux@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

