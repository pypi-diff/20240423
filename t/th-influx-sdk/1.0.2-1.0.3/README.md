# Comparing `tmp/th-influx-sdk-1.0.2.tar.gz` & `tmp/th-influx-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.2.tar", last modified: Fri Apr 19 07:17:56 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.3.tar", last modified: Tue Apr 23 01:28:43 2024, max compression
```

## Comparing `th-influx-sdk-1.0.2.tar` & `th-influx-sdk-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:17:56.160298 th-influx-sdk-1.0.2/
--rw-rw-rw-   0        0        0      300 2024-04-19 07:17:56.158303 th-influx-sdk-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:17:56.148346 th-influx-sdk-1.0.2/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.2/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0     6934 2024-04-19 05:42:36.000000 th-influx-sdk-1.0.2/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:17:56.160298 th-influx-sdk-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-19 07:17:42.000000 th-influx-sdk-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:17:56.156701 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      300 2024-04-19 07:17:56.000000 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-19 07:17:56.000000 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:17:56.000000 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-19 07:17:56.000000 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:17:56.000000 th-influx-sdk-1.0.2/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.624300 th-influx-sdk-1.0.3/
+-rw-rw-rw-   0        0        0      300 2024-04-23 01:28:43.622306 th-influx-sdk-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.611364 th-influx-sdk-1.0.3/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.3/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0    18398 2024-04-23 01:19:12.000000 th-influx-sdk-1.0.3/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 01:28:43.624300 th-influx-sdk-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-23 01:26:03.000000 th-influx-sdk-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.620347 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.2/setup.py` & `th-influx-sdk-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.2',
+    version='1.0.3',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
```

