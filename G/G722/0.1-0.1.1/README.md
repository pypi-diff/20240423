# Comparing `tmp/g722-0.1.tar.gz` & `tmp/g722-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g722-0.1.tar", last modified: Mon Apr 22 23:19:41 2024, max compression
+gzip compressed data, was "g722-0.1.1.tar", last modified: Mon Apr 22 23:29:32 2024, max compression
```

## Comparing `g722-0.1.tar` & `g722-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:41.110186 g722-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:41.110186 g722-0.1/G722.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-22 23:19:41.000000 g722-0.1/G722.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 23:19:41.000000 g722-0.1/G722.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:41.000000 g722-0.1/G722.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:19:41.000000 g722-0.1/G722.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:19:41.000000 g722-0.1/G722.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 23:19:27.000000 g722-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 23:19:27.000000 g722-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-22 23:19:41.110186 g722-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 23:19:27.000000 g722-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-22 23:19:27.000000 g722-0.1/g722.h
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 23:19:27.000000 g722-0.1/g722_codec.h
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-22 23:19:27.000000 g722-0.1/g722_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-22 23:19:27.000000 g722-0.1/g722_decode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:19:27.000000 g722-0.1/g722_decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-22 23:19:27.000000 g722-0.1/g722_encode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:19:27.000000 g722-0.1/g722_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 23:19:27.000000 g722-0.1/g722_private.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:41.110186 g722-0.1/python/
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-04-22 23:19:27.000000 g722-0.1/python/G722_mod.c
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:19:27.000000 g722-0.1/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 23:19:27.000000 g722-0.1/python/symbols.map
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:41.110186 g722-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 23:19:27.000000 g722-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:32.540482 g722-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:32.540482 g722-0.1.1/G722.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-22 23:29:32.000000 g722-0.1.1/G722.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 23:29:32.000000 g722-0.1.1/G722.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:29:32.000000 g722-0.1.1/G722.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:29:32.000000 g722-0.1.1/G722.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:29:32.000000 g722-0.1.1/G722.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 23:29:25.000000 g722-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 23:29:25.000000 g722-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-22 23:29:32.540482 g722-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 23:29:25.000000 g722-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-22 23:29:25.000000 g722-0.1.1/g722.h
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 23:29:25.000000 g722-0.1.1/g722_codec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-22 23:29:25.000000 g722-0.1.1/g722_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-22 23:29:25.000000 g722-0.1.1/g722_decode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:29:25.000000 g722-0.1.1/g722_decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-22 23:29:25.000000 g722-0.1.1/g722_encode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 23:29:25.000000 g722-0.1.1/g722_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 23:29:25.000000 g722-0.1.1/g722_private.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:29:32.540482 g722-0.1.1/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-04-22 23:29:25.000000 g722-0.1.1/python/G722_mod.c
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:29:25.000000 g722-0.1.1/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 23:29:25.000000 g722-0.1.1/python/symbols.map
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:29:32.540482 g722-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-22 23:29:25.000000 g722-0.1.1/setup.py
```

### Comparing `g722-0.1/G722.egg-info/PKG-INFO` & `g722-0.1.1/G722.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: G722
-Version: 0.1
+Version: 0.1.1
 Summary: This is a package for G.722 module
 Home-page: https://github.com/sippy/libg722
 Author: Maksym Sobolyev
 Author-email: sobomax@sippysoft.com
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `g722-0.1/LICENSE` & `g722-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g722-0.1/PKG-INFO` & `g722-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: G722
-Version: 0.1
+Version: 0.1.1
 Summary: This is a package for G.722 module
 Home-page: https://github.com/sippy/libg722
 Author: Maksym Sobolyev
 Author-email: sobomax@sippysoft.com
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `g722-0.1/README.md` & `g722-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722.h` & `g722-0.1.1/g722.h`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_common.h` & `g722-0.1.1/g722_common.h`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_decode.c` & `g722-0.1.1/g722_decode.c`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_decoder.h` & `g722-0.1.1/g722_decoder.h`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_encode.c` & `g722-0.1.1/g722_encode.c`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_encoder.h` & `g722-0.1.1/g722_encoder.h`

 * *Files identical despite different names*

### Comparing `g722-0.1/g722_private.h` & `g722-0.1.1/g722_private.h`

 * *Files identical despite different names*

### Comparing `g722-0.1/python/G722_mod.c` & `g722-0.1.1/python/G722_mod.c`

 * *Files identical despite different names*

### Comparing `g722-0.1/setup.py` & `g722-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 requirements = [x.strip() for x in open(mod_dir + "requirements.txt", "r").readlines()]
 with open(src_dir + "README.md", "r") as fh:
     long_description = fh.read()
 
 kwargs = {
       'name':mod_name,
-      'version':'0.1',
+      'version':'0.1.1',
       'description':'This is a package for G.722 module',
       'long_description': long_description,
       'long_description_content_type': "text/markdown",
       'author':'Maksym Sobolyev',
       'author_email':'sobomax@sippysoft.com',
       'url':'https://github.com/sippy/libg722',
       'ext_modules': [module1, module2],
       'python_requires': '>=3.10',
       'install_requires': requirements,
       'classifiers': [
-            'License :: OSI Approved :: BSD License',
-            'Operating System :: POSIX',
+            'License :: Public Domain',
+            'Operating System :: OS Independent',
             'Programming Language :: C',
             'Programming Language :: Python'
       ]
 }
 
 setup (**kwargs)
```

