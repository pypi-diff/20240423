# Comparing `tmp/thriftify-0.1.1.tar.gz` & `tmp/thriftify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thriftify-0.1.1.tar", last modified: Sun Apr 21 07:39:06 2024, max compression
+gzip compressed data, was "thriftify-0.1.2.tar", last modified: Tue Apr 23 04:55:28 2024, max compression
```

## Comparing `thriftify-0.1.1.tar` & `thriftify-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-21 07:39:06.951556 thriftify-0.1.1/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 thriftify-0.1.1/LICENSE
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 thriftify-0.1.1/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-21 07:39:06.951451 thriftify-0.1.1/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      911 2024-04-20 07:58:15.000000 thriftify-0.1.1/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 thriftify-0.1.1/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-21 07:39:06.949645 thriftify-0.1.1/bin/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      105 2024-04-21 07:30:10.000000 thriftify-0.1.1/bin/thriftify
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-21 07:39:06.951604 thriftify-0.1.1/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1081 2024-04-21 07:39:03.000000 thriftify-0.1.1/setup.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-21 07:39:06.950150 thriftify-0.1.1/thriftify/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       33 2024-04-21 07:37:23.000000 thriftify-0.1.1/thriftify/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)    14912 2024-04-21 07:18:01.000000 thriftify-0.1.1/thriftify/thriftify.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-21 07:39:06.951279 thriftify-0.1.1/thriftify.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      340 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/entry_points.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:07:29.000000 thriftify-0.1.1/thriftify.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-21 07:39:06.000000 thriftify-0.1.1/thriftify.egg-info/top_level.txt
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.562488 thriftify-0.1.2/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 thriftify-0.1.2/LICENSE
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 thriftify-0.1.2/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 04:55:28.562376 thriftify-0.1.2/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      911 2024-04-20 07:58:15.000000 thriftify-0.1.2/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1064 2024-04-21 07:43:24.000000 thriftify-0.1.2/README.rst
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-23 04:55:28.562796 thriftify-0.1.2/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1108 2024-04-23 04:55:23.000000 thriftify-0.1.2/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.560810 thriftify-0.1.2/thriftify/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       33 2024-04-22 17:04:42.000000 thriftify-0.1.2/thriftify/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       56 2024-04-22 07:42:37.000000 thriftify-0.1.2/thriftify/command_line.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)    14959 2024-04-23 04:53:06.000000 thriftify-0.1.2/thriftify/thriftify.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.562215 thriftify-0.1.2/thriftify.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      352 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/entry_points.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:07:29.000000 thriftify-0.1.2/thriftify.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/top_level.txt
```

### Comparing `thriftify-0.1.1/LICENSE` & `thriftify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.1/PKG-INFO` & `thriftify-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftify
-Version: 0.1.1
+Version: 0.1.2
 Summary: Converts xlsx files into thrift binary or json blobs
 Home-page: http://github.com/ohthepain/thriftify
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Platform: UNKNOWN
```

### Comparing `thriftify-0.1.1/README.md` & `thriftify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.1/setup.py` & `thriftify-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='thriftify',
-      version='0.1.1',
+      version='0.1.2',
       description='Converts xlsx files into thrift binary or json blobs',
       long_description='Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.',
       long_description_content_type='text/x-rst',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
@@ -19,13 +19,15 @@
       install_requires=[
             'openpyxl',
             'datetime',
             'thrift',
             'argparse',
             'datetime',
       ],
-      scripts=['bin/thriftify'],
+      # scripts=['bin/thriftify_cli'],
       entry_points = {
-        'console_scripts': ['thriftify=thriftify.command_line:main'],
+        'console_scripts': [
+          'thriftify=thriftify.command_line:main',
+        ],
       },
       zip_safe=False)
```

### Comparing `thriftify-0.1.1/thriftify/thriftify.py` & `thriftify-0.1.2/thriftify/thriftify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import sys, os
 import importlib
+import argparse
+import datetime
+
 import thrift
 from thrift.transport import TTransport
 from thrift.Thrift import TType
 from openpyxl import Workbook
 from openpyxl import load_workbook
-import argparse
-import datetime
 import openpyxl
 
 parser = argparse.ArgumentParser(description='Excel converter')
 parser.add_argument('--namespace', help='namespace from thrift file')
 parser.add_argument('--thrift_protocol', choices=('TCompactProtocol', 'TJSONProtocol', 'TBinaryProtocol'), default='TJSONProtocol')
 parser.add_argument('--gen_py', default='')
 parser.add_argument('--output', default='config.bin')
@@ -379,21 +380,22 @@
         os.makedirs(directory)
 
 # Globals
 typeEntries = {}
 Data = {}
 enums = {}
 
-def main():
-	Log("awesome")
-	sys.path.append(args.gen_py)
+import inspect
+
+def thriftify():
+	Log('Hi from thriftify: Loading <%s> from: <%s>' % (args.namespace, args.gen_py))
+
+	sys.path.append('%s' % (args.gen_py))
 	ConfigModule = importlib.import_module('%s.ttypes' % (args.namespace))
-	ConfigConstants = importlib.import_module('%s.constants' % (args.namespace))
-	dataClass = getattr(ConfigModule, args.class_name)
-	globals()['Data'] = dataClass()
+	globals()['Data'] = ConfigModule.ConfigData()
 	Data = globals()['Data']
 
 	sheetInfo = None
 
 	if args.enums:
 		globals()['enums'] = parseEnums(enums)
 	globals()['typeEntries'] = makeTypeEntries(Data)
@@ -414,26 +416,28 @@
 
 	transport = TTransport.TMemoryBuffer()
 	ThriftProtocol = getattr(importlib.import_module("thrift.protocol.%s" % (args.thrift_protocol)), args.thrift_protocol)
 	protocol = ThriftProtocol(transport)
 	Data.schemaVersionId = 1
 	Data.write(protocol)
 
+	# Write output file
 	configPath = args.output
 	buf = transport.getvalue()
 	with open(configPath, 'wb') as f:
 		f.write(buf)
 
+	# Read and validate
 	buf = None
 
 	with open(configPath, 'rb') as f:
 		buf = f.read()
 
 	transport = TTransport.TMemoryBuffer(buf)
 	protocol = ThriftProtocol(transport)
 	Data = None
-	Data = dataClass()
+	# Data = dataClass()
+	Data = ConfigModule.ConfigData()
 	Data.read(protocol)
 	Data.validate()
 
-main()
-Log("awesomedunn")
+thriftify()
```

### Comparing `thriftify-0.1.1/thriftify.egg-info/PKG-INFO` & `thriftify-0.1.2/thriftify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftify
-Version: 0.1.1
+Version: 0.1.2
 Summary: Converts xlsx files into thrift binary or json blobs
 Home-page: http://github.com/ohthepain/thriftify
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Platform: UNKNOWN
```

