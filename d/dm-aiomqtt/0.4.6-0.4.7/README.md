# Comparing `tmp/dm_aiomqtt-0.4.6.tar.gz` & `tmp/dm_aiomqtt-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.6.tar", last modified: Fri Apr 19 20:59:57 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.7.tar", last modified: Tue Apr 23 07:35:53 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.6.tar` & `dm_aiomqtt-0.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:59:57.674144 dm_aiomqtt-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 20:59:57.674144 dm_aiomqtt-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-19 20:59:48.000000 dm_aiomqtt-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:59:57.670143 dm_aiomqtt-0.4.6/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 20:59:48.000000 dm_aiomqtt-0.4.6/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-19 20:59:48.000000 dm_aiomqtt-0.4.6/dm_aiomqtt/dm_aiomqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 20:59:48.000000 dm_aiomqtt-0.4.6/dm_aiomqtt/message_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:59:57.674144 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:59:57.674144 dm_aiomqtt-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 20:59:57.000000 dm_aiomqtt-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/dm_aiomqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/message_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/setup.py
```

### Comparing `dm_aiomqtt-0.4.6/PKG-INFO` & `dm_aiomqtt-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.6
+Version: 0.4.7
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: dm-logger==0.5.2
 Requires-Dist: aiomqtt==2.0.0
+Requires-Dist: aiofiles==23.2.1
 
 # DM-aiomqtt
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomqtt)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomqtt)
```

### Comparing `dm_aiomqtt-0.4.6/README.md` & `dm_aiomqtt-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.6/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.7/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.6/dm_aiomqtt/message_db.py` & `dm_aiomqtt-0.4.7/dm_aiomqtt/message_db.py`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.6/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.6
+Version: 0.4.7
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: dm-logger==0.5.2
 Requires-Dist: aiomqtt==2.0.0
+Requires-Dist: aiofiles==23.2.1
 
 # DM-aiomqtt
 
 ## Urls
 
 * [PyPI](https://pypi.org/project/dm-aiomqtt)
 * [GitHub](https://github.com/DIMKA4621/dm-aiomqtt)
```

### Comparing `dm_aiomqtt-0.4.6/setup.py` & `dm_aiomqtt-0.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.6',
+    version='v0.4.7',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
     install_requires=[
         'dm-logger==0.5.2',
-        'aiomqtt==2.0.0'
+        'aiomqtt==2.0.0',
+        'aiofiles==23.2.1'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     keywords='dm aiomqtt',
```

