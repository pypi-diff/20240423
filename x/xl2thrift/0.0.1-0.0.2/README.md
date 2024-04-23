# Comparing `tmp/xl2thrift-0.0.1.tar.gz` & `tmp/xl2thrift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2thrift-0.0.1.tar", last modified: Tue Apr 23 12:18:16 2024, max compression
+gzip compressed data, was "xl2thrift-0.0.2.tar", last modified: Tue Apr 23 13:13:54 2024, max compression
```

## Comparing `xl2thrift-0.0.1.tar` & `xl2thrift-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 12:18:16.042853 xl2thrift-0.0.1/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 xl2thrift-0.0.1/LICENSE
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 xl2thrift-0.0.1/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      688 2024-04-23 12:18:16.042734 xl2thrift-0.0.1/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1061 2024-04-23 10:17:36.000000 xl2thrift-0.0.1/README.rst
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-23 12:18:16.042902 xl2thrift-0.0.1/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1109 2024-04-23 10:16:18.000000 xl2thrift-0.0.1/setup.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 12:18:16.041199 xl2thrift-0.0.1/xl2thrift/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       42 2024-04-23 07:42:48.000000 xl2thrift-0.0.1/xl2thrift/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       73 2024-04-23 07:44:01.000000 xl2thrift-0.0.1/xl2thrift/command_line.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)    16389 2024-04-23 12:07:04.000000 xl2thrift-0.0.1/xl2thrift/thriftExcelTools.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 12:18:16.042567 xl2thrift-0.0.1/xl2thrift.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      688 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      349 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/entry_points.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 10:18:35.000000 xl2thrift-0.0.1/xl2thrift.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-23 12:18:16.000000 xl2thrift-0.0.1/xl2thrift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.381543 xl2thrift-0.0.2/xl2thrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/thriftExcelTools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.381543 xl2thrift-0.0.2/xl2thrift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/top_level.txt
```

### Comparing `xl2thrift-0.0.1/LICENSE` & `xl2thrift-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2thrift-0.0.1/PKG-INFO` & `xl2thrift-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: xl2thrift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts xlsx files into thrift files that can be deserialized in many programming languages
 Home-page: http://github.com/ohthepain/xl2thrift
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: openpyxl
+Requires-Dist: datetime
+Requires-Dist: thrift
+Requires-Dist: argparse
+Requires-Dist: datetime
 
 Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.
-
```

### Comparing `xl2thrift-0.0.1/README.rst` & `xl2thrift-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `xl2thrift-0.0.1/setup.py` & `xl2thrift-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='xl2thrift',
-      version='0.0.1',
+      version='0.0.2',
       description='Converts xlsx files into thrift files that can be deserialized in many programming languages',
       long_description='Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.',
       long_description_content_type='text/x-rst',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

### Comparing `xl2thrift-0.0.1/xl2thrift/thriftExcelTools.py` & `xl2thrift-0.0.2/xl2thrift/thriftExcelTools.py`

 * *Files identical despite different names*

### Comparing `xl2thrift-0.0.1/xl2thrift.egg-info/PKG-INFO` & `xl2thrift-0.0.2/xl2thrift.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: xl2thrift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts xlsx files into thrift files that can be deserialized in many programming languages
 Home-page: http://github.com/ohthepain/xl2thrift
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: openpyxl
+Requires-Dist: datetime
+Requires-Dist: thrift
+Requires-Dist: argparse
+Requires-Dist: datetime
 
 Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.
-
```

