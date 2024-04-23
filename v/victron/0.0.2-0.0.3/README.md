# Comparing `tmp/victron-0.0.2.tar.gz` & `tmp/victron-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victron-0.0.2.tar", last modified: Sat Apr 20 18:19:35 2024, max compression
+gzip compressed data, was "victron-0.0.3.tar", last modified: Tue Apr 23 20:55:28 2024, max compression
```

## Comparing `victron-0.0.2.tar` & `victron-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.742142 victron-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-20 18:19:29.000000 victron-0.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-20 18:19:29.000000 victron-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-20 18:19:35.742142 victron-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-20 18:19:29.000000 victron-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-20 18:19:35.743142 victron-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-20 18:19:29.000000 victron-0.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-20 18:19:29.000000 victron-0.0.2/versioneer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.741142 victron-0.0.2/victron/
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-20 18:19:29.000000 victron-0.0.2/victron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-20 18:19:35.743142 victron-0.0.2/victron/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-20 18:19:29.000000 victron-0.0.2/victron/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2024-04-20 18:19:29.000000 victron-0.0.2/victron/victron.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 18:19:35.742142 victron-0.0.2/victron.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      296 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 18:19:35.000000 victron-0.0.2/victron.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.347638 victron-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-23 20:55:22.000000 victron-0.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-23 20:55:22.000000 victron-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-23 20:55:28.347638 victron-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-23 20:55:22.000000 victron-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-23 20:55:28.348638 victron-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-23 20:55:22.000000 victron-0.0.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-23 20:55:22.000000 victron-0.0.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.346638 victron-0.0.3/victron/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-23 20:55:22.000000 victron-0.0.3/victron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-23 20:55:28.348638 victron-0.0.3/victron/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-23 20:55:22.000000 victron-0.0.3/victron/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-23 20:55:22.000000 victron-0.0.3/victron/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2024-04-23 20:55:22.000000 victron-0.0.3/victron/victron.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.347638 victron-0.0.3/victron.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/top_level.txt
```

### Comparing `victron-0.0.2/LICENSE` & `victron-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `victron-0.0.2/PKG-INFO` & `victron-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.2
+Version: 0.0.3
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `victron-0.0.2/README.md` & `victron-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `victron-0.0.2/setup.cfg` & `victron-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `victron-0.0.2/versioneer.py` & `victron-0.0.3/versioneer.py`

 * *Files identical despite different names*

### Comparing `victron-0.0.2/victron.egg-info/PKG-INFO` & `victron-0.0.3/victron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.2
+Version: 0.0.3
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

