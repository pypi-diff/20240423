# Comparing `tmp/thriftify-0.1.4.tar.gz` & `tmp/thriftify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thriftify-0.1.4.tar", last modified: Tue Apr 23 07:44:03 2024, max compression
+gzip compressed data, was "thriftify-0.1.5.tar", last modified: Tue Apr 23 09:38:54 2024, max compression
```

## Comparing `thriftify-0.1.4.tar` & `thriftify-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:44:03.411706 thriftify-0.1.4/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 thriftify-0.1.4/LICENSE
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 thriftify-0.1.4/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 07:44:03.411583 thriftify-0.1.4/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      911 2024-04-20 07:58:15.000000 thriftify-0.1.4/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1064 2024-04-21 07:43:24.000000 thriftify-0.1.4/README.rst
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-23 07:44:03.411757 thriftify-0.1.4/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1108 2024-04-23 07:37:46.000000 thriftify-0.1.4/setup.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:44:03.410497 thriftify-0.1.4/thriftify/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       42 2024-04-23 07:42:48.000000 thriftify-0.1.4/thriftify/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       73 2024-04-23 07:44:01.000000 thriftify-0.1.4/thriftify/command_line.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)    14963 2024-04-23 07:28:32.000000 thriftify-0.1.4/thriftify/thriftExcelTools.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:44:03.411429 thriftify-0.1.4/thriftify.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      359 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/entry_points.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:07:29.000000 thriftify-0.1.4/thriftify.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-23 07:44:03.000000 thriftify-0.1.4/thriftify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:38:54.081838 thriftify-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 09:38:50.000000 thriftify-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 09:38:50.000000 thriftify-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 09:38:54.081838 thriftify-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 09:38:50.000000 thriftify-0.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:38:54.081838 thriftify-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 09:38:50.000000 thriftify-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:38:54.077837 thriftify-0.1.5/thriftify/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 09:38:50.000000 thriftify-0.1.5/thriftify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 09:38:50.000000 thriftify-0.1.5/thriftify/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-23 09:38:50.000000 thriftify-0.1.5/thriftify/thriftExcelTools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:38:54.081838 thriftify-0.1.5/thriftify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:38:54.000000 thriftify-0.1.5/thriftify.egg-info/top_level.txt
```

### Comparing `thriftify-0.1.4/LICENSE` & `thriftify-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.4/README.rst` & `thriftify-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.4/setup.py` & `thriftify-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='thriftify',
-      version='0.1.4',
+      version='0.1.5',
       description='Converts xlsx files into thrift binary or json blobs',
       long_description='Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.',
       long_description_content_type='text/x-rst',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

### Comparing `thriftify-0.1.4/thriftify/thriftExcelTools.py` & `thriftify-0.1.5/thriftify/thriftExcelTools.py`

 * *Files identical despite different names*

