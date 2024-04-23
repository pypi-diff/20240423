# Comparing `tmp/basicbedrock-0.1.4.tar.gz` & `tmp/basicbedrock-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.4.tar", last modified: Mon Apr 22 22:01:59 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.5.tar", last modified: Tue Apr 23 14:52:00 2024, max compression
```

## Comparing `basicbedrock-0.1.4.tar` & `basicbedrock-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.015299 basicbedrock-0.1.4/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.4/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-22 22:01:59.015028 basicbedrock-0.1.4/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.4/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-22 22:01:13.000000 basicbedrock-0.1.4/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-22 22:01:59.015427 basicbedrock-0.1.4/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.010460 basicbedrock-0.1.4/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.011499 basicbedrock-0.1.4/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-22 22:01:13.000000 basicbedrock-0.1.4/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    16155 2024-04-11 01:17:00.000000 basicbedrock-0.1.4/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.013926 basicbedrock-0.1.4/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2984 2024-04-22 22:00:00.000000 basicbedrock-0.1.4/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.4/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.4/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.4/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2315 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.4/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.014725 basicbedrock-0.1.4/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.014086 basicbedrock-0.1.4/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.4/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.165076 basicbedrock-0.1.5/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.5/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-23 14:52:00.164795 basicbedrock-0.1.5/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.5/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-23 14:51:35.000000 basicbedrock-0.1.5/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-23 14:52:00.165142 basicbedrock-0.1.5/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.158762 basicbedrock-0.1.5/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.159798 basicbedrock-0.1.5/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-23 14:50:30.000000 basicbedrock-0.1.5/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    16145 2024-04-23 14:50:11.000000 basicbedrock-0.1.5/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.163019 basicbedrock-0.1.5/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2984 2024-04-22 22:00:00.000000 basicbedrock-0.1.5/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.5/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.5/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.5/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2315 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.5/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.164423 basicbedrock-0.1.5/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.163235 basicbedrock-0.1.5/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.5/test/tests.py
```

### Comparing `basicbedrock-0.1.4/LICENSE` & `basicbedrock-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/PKG-INFO` & `basicbedrock-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.4
+Version: 0.1.5
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.4/README.md` & `basicbedrock-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/pyproject.toml` & `basicbedrock-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.4/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.5/src/basicbedrock/basicbedrock.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 from models import *
 
 
 class BasicBedrock(object):
     def __init__(self, session: boto3.session.Session = None, **kwargs):
         """
         Creates an instance of basic bedrock.
-        session param is optional.  If omitted, a default session will be used.
+        session param is optional.  If omitted, a default session constructor will be used.
         Right now, the only kwargs supported are a param dictionary.
         Param dicts are in the format of {'top_p': float, 'top_k': int, 'temp': float, 'max_tokens': int}
         :param session: the boto3 session to use for creating the basic bedrock instance
         :param kwargs: kwargs used are in the format of {'top_p': float, 'top_k': int, 'temp': float, 'max_tokens': int}
         """
         if not session:
-            warnings.warn('No session provided, attemtping to use "default" profile', category=RuntimeWarning)
-            session = boto3.session.Session(profile_name='default')
+            warnings.warn('No session provided, attempting to use "default" profile', category=RuntimeWarning)
+            session = boto3.session.Session()
         self.client = session.client("bedrock-runtime")
         self._default_k = 100
         self._default_p = .5
         self._default_t = .5
         self._default_n = 150
         self._default_stop = []
         # intialize params to default values
```

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.5/src/basicbedrock/models/__init__.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/ai21.py` & `basicbedrock-0.1.5/src/basicbedrock/models/ai21.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.5/src/basicbedrock/models/amazon.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.1.5/src/basicbedrock/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.5/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/cohere.py` & `basicbedrock-0.1.5/src/basicbedrock/models/cohere.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.5/src/basicbedrock/models/meta.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.5/src/basicbedrock/models/mistral.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.5/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.4
+Version: 0.1.5
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.4/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.5/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.4/test/tests.py` & `basicbedrock-0.1.5/test/tests.py`

 * *Files identical despite different names*

