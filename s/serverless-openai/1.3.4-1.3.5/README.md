# Comparing `tmp/serverless_openai-1.3.4.tar.gz` & `tmp/serverless_openai-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless_openai-1.3.4.tar", last modified: Tue Apr 23 10:14:41 2024, max compression
+gzip compressed data, was "serverless_openai-1.3.5.tar", last modified: Tue Apr 23 10:46:06 2024, max compression
```

## Comparing `serverless_openai-1.3.4.tar` & `serverless_openai-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/serverless_openai/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/serverless_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/serverless_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/serverless_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/setup.py
```

### Comparing `serverless_openai-1.3.4/PKG-INFO` & `serverless_openai-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.4
+Version: 1.3.5
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.4/serverless_openai/apis.py` & `serverless_openai-1.3.5/serverless_openai/apis.py`

 * *Files identical despite different names*

### Comparing `serverless_openai-1.3.4/serverless_openai/helpers.py` & `serverless_openai-1.3.5/serverless_openai/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,24 @@
     def check_url(cls, v, values):
         if isinstance(v, str):
             try:
                 TypeAdapter(HttpUrl).validate_python(v)
                 return v
             except ValidationError:
                 return encode_image(v)
-        return v
+        elif isinstance(v, list):
+            vlist = []
+            for vi in v:
+                try:
+                    TypeAdapter(HttpUrl).validate_python(v)
+                    vlist.append(vi)
+                except ValidationError:
+                    vlist.append(encode_image(vi))
+            return vlist
+
     class Config:
         arbitrary_types_allowed = True
 
 class EmbeddingModels(str, ExtendedEnum):
     te_ada2 : str = "text-embedding-ada-002"
     te3_small: str = "text-embedding-3-small"
     te3_large: str = "text-embedding-3-large"
```

### Comparing `serverless_openai-1.3.4/serverless_openai.egg-info/PKG-INFO` & `serverless_openai-1.3.5/serverless_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.4
+Version: 1.3.5
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.4/setup.py` & `serverless_openai-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.4'
+VERSION = '1.3.5'
 DESCRIPTION = "A package for using Openai in serverless environment"
 LONG_DESCRIPTION = 'A package for using Openai with scraping and etc. in serverless application such as AWS Lambda and GCP Cloud Function'
 
 # Setting up
 setup(
     name="serverless_openai",
     version=VERSION,
```

