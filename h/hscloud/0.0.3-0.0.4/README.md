# Comparing `tmp/hscloud-0.0.3.tar.gz` & `tmp/hscloud-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.3.tar", last modified: Mon Apr 22 09:39:18 2024, max compression
+gzip compressed data, was "hscloud-0.0.4.tar", last modified: Mon Apr 22 11:35:12 2024, max compression
```

## Comparing `hscloud-0.0.3.tar` & `hscloud-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:39:18.553190 hscloud-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-22 09:39:18.548193 hscloud-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-22 09:39:18.540190 hscloud-0.0.3/hscloud/
--rw-rw-rw-   0        0        0     2054 2024-04-22 09:25:12.000000 hscloud-0.0.3/hscloud/__init__.py
--rw-rw-rw-   0        0        0     1987 2024-04-22 09:01:00.000000 hscloud-0.0.3/hscloud/helpers.py
--rw-rw-rw-   0        0        0     1555 2024-04-22 09:23:07.000000 hscloud-0.0.3/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:39:18.546193 hscloud-0.0.3/hscloud.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-22 09:39:18.000000 hscloud-0.0.3/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-22 09:39:18.000000 hscloud-0.0.3/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:39:18.000000 hscloud-0.0.3/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 09:39:18.000000 hscloud-0.0.3/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 09:39:18.553190 hscloud-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-22 09:39:07.000000 hscloud-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.742620 hscloud-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-22 11:35:12.741620 hscloud-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.731616 hscloud-0.0.4/hscloud/
+-rw-rw-rw-   0        0        0     2054 2024-04-22 09:25:12.000000 hscloud-0.0.4/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     1987 2024-04-22 09:01:00.000000 hscloud-0.0.4/hscloud/helpers.py
+-rw-rw-rw-   0        0        0     1374 2024-04-22 11:32:20.000000 hscloud-0.0.4/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.739616 hscloud-0.0.4/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 11:35:12.742620 hscloud-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-22 11:34:42.000000 hscloud-0.0.4/setup.py
```

### Comparing `hscloud-0.0.3/hscloud/__init__.py` & `hscloud-0.0.4/hscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.3/hscloud/helpers.py` & `hscloud-0.0.4/hscloud/helpers.py`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.3/setup.py` & `hscloud-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="hscloud",
-    version="0.0.3",
+    version="0.0.4",
     author="kane",
     author_email="wang.xiangtao@qq.com",
     description="A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clement-bonnet/medium-first-package",
     packages=find_packages(),
```

