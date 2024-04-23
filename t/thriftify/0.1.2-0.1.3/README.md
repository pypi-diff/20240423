# Comparing `tmp/thriftify-0.1.2.tar.gz` & `tmp/thriftify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thriftify-0.1.2.tar", last modified: Tue Apr 23 04:55:28 2024, max compression
+gzip compressed data, was "thriftify-0.1.3.tar", last modified: Tue Apr 23 07:35:33 2024, max compression
```

## Comparing `thriftify-0.1.2.tar` & `thriftify-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.562488 thriftify-0.1.2/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 thriftify-0.1.2/LICENSE
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 thriftify-0.1.2/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 04:55:28.562376 thriftify-0.1.2/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      911 2024-04-20 07:58:15.000000 thriftify-0.1.2/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1064 2024-04-21 07:43:24.000000 thriftify-0.1.2/README.rst
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-23 04:55:28.562796 thriftify-0.1.2/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)     1108 2024-04-23 04:55:23.000000 thriftify-0.1.2/setup.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.560810 thriftify-0.1.2/thriftify/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       33 2024-04-22 17:04:42.000000 thriftify-0.1.2/thriftify/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       56 2024-04-22 07:42:37.000000 thriftify-0.1.2/thriftify/command_line.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)    14959 2024-04-23 04:53:06.000000 thriftify-0.1.2/thriftify/thriftify.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 04:55:28.562215 thriftify-0.1.2/thriftify.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      352 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/entry_points.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:07:29.000000 thriftify-0.1.2/thriftify.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-23 04:55:28.000000 thriftify-0.1.2/thriftify.egg-info/top_level.txt
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:35:33.402936 thriftify-0.1.3/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1071 2024-04-20 07:16:43.000000 thriftify-0.1.3/LICENSE
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 thriftify-0.1.3/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 07:35:33.402788 thriftify-0.1.3/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      911 2024-04-20 07:58:15.000000 thriftify-0.1.3/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1064 2024-04-21 07:43:24.000000 thriftify-0.1.3/README.rst
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-23 07:35:33.402993 thriftify-0.1.3/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)     1108 2024-04-23 07:35:27.000000 thriftify-0.1.3/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:35:33.401221 thriftify-0.1.3/thriftify/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       33 2024-04-22 17:04:42.000000 thriftify-0.1.3/thriftify/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       73 2024-04-23 07:33:44.000000 thriftify-0.1.3/thriftify/command_line.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)    14963 2024-04-23 07:28:32.000000 thriftify-0.1.3/thriftify/thriftExcelTools.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-23 07:35:33.402561 thriftify-0.1.3/thriftify.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      648 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      359 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       59 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/entry_points.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-21 07:07:29.000000 thriftify-0.1.3/thriftify.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       43 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       10 2024-04-23 07:35:33.000000 thriftify-0.1.3/thriftify.egg-info/top_level.txt
```

### Comparing `thriftify-0.1.2/LICENSE` & `thriftify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.2/PKG-INFO` & `thriftify-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Converts xlsx files into thrift binary or json blobs
 Home-page: http://github.com/ohthepain/thriftify
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Platform: UNKNOWN
```

### Comparing `thriftify-0.1.2/README.md` & `thriftify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.2/README.rst` & `thriftify-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `thriftify-0.1.2/setup.py` & `thriftify-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='thriftify',
-      version='0.1.2',
+      version='0.1.3',
       description='Converts xlsx files into thrift binary or json blobs',
       long_description='Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.',
       long_description_content_type='text/x-rst',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

### Comparing `thriftify-0.1.2/thriftify/thriftify.py` & `thriftify-0.1.3/thriftify/thriftExcelTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 # Globals
 typeEntries = {}
 Data = {}
 enums = {}
 
 import inspect
 
-def thriftify():
+def convertXlsx():
 	Log('Hi from thriftify: Loading <%s> from: <%s>' % (args.namespace, args.gen_py))
 
 	sys.path.append('%s' % (args.gen_py))
 	ConfigModule = importlib.import_module('%s.ttypes' % (args.namespace))
 	globals()['Data'] = ConfigModule.ConfigData()
 	Data = globals()['Data']
 
@@ -436,8 +436,8 @@
 	protocol = ThriftProtocol(transport)
 	Data = None
 	# Data = dataClass()
 	Data = ConfigModule.ConfigData()
 	Data.read(protocol)
 	Data.validate()
 
-thriftify()
+# thriftify()
```

### Comparing `thriftify-0.1.2/thriftify.egg-info/PKG-INFO` & `thriftify-0.1.3/thriftify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Converts xlsx files into thrift binary or json blobs
 Home-page: http://github.com/ohthepain/thriftify
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Platform: UNKNOWN
```

