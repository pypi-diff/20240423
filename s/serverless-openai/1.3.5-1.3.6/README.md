# Comparing `tmp/serverless_openai-1.3.5.tar.gz` & `tmp/serverless_openai-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless_openai-1.3.5.tar", last modified: Tue Apr 23 10:46:06 2024, max compression
+gzip compressed data, was "serverless_openai-1.3.6.tar", last modified: Tue Apr 23 11:00:04 2024, max compression
```

## Comparing `serverless_openai-1.3.5.tar` & `serverless_openai-1.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/serverless_openai/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/serverless_openai/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/serverless_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 10:46:06.000000 serverless_openai-1.3.5/serverless_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:46:06.728085 serverless_openai-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 10:46:02.000000 serverless_openai-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:00:04.303040 serverless_openai-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 11:00:04.303040 serverless_openai-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:00:00.000000 serverless_openai-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:00:04.303040 serverless_openai-1.3.6/serverless_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 11:00:00.000000 serverless_openai-1.3.6/serverless_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 11:00:00.000000 serverless_openai-1.3.6/serverless_openai/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-23 11:00:00.000000 serverless_openai-1.3.6/serverless_openai/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:00:04.303040 serverless_openai-1.3.6/serverless_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 11:00:04.000000 serverless_openai-1.3.6/serverless_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 11:00:04.000000 serverless_openai-1.3.6/serverless_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:00:04.000000 serverless_openai-1.3.6/serverless_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 11:00:04.000000 serverless_openai-1.3.6/serverless_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 11:00:04.000000 serverless_openai-1.3.6/serverless_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:00:04.303040 serverless_openai-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 11:00:00.000000 serverless_openai-1.3.6/setup.py
```

### Comparing `serverless_openai-1.3.5/PKG-INFO` & `serverless_openai-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.5/serverless_openai/apis.py` & `serverless_openai-1.3.6/serverless_openai/apis.py`

 * *Files identical despite different names*

### Comparing `serverless_openai-1.3.5/serverless_openai/helpers.py` & `serverless_openai-1.3.6/serverless_openai/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     dalle_3 : str = "dall-e-3"
 
 class VisionModels(str, ExtendedEnum):
     gpt4_vision : str = "gpt-4-vision-preview"
 
 class VisionMessage(BaseModel):
     text: str
-    image: Union[str, np.ndarray]
+    image: Union[str, np.ndarray, List[str]]
     role: Roles = Roles.user
     
     @validator('image', always=True)
     def check_url(cls, v, values):
         if isinstance(v, str):
             try:
                 TypeAdapter(HttpUrl).validate_python(v)
@@ -64,15 +64,15 @@
             for vi in v:
                 try:
                     TypeAdapter(HttpUrl).validate_python(v)
                     vlist.append(vi)
                 except ValidationError:
                     vlist.append(encode_image(vi))
             return vlist
-
+        return v
     class Config:
         arbitrary_types_allowed = True
 
 class EmbeddingModels(str, ExtendedEnum):
     te_ada2 : str = "text-embedding-ada-002"
     te3_small: str = "text-embedding-3-small"
     te3_large: str = "text-embedding-3-large"
```

### Comparing `serverless_openai-1.3.5/serverless_openai.egg-info/PKG-INFO` & `serverless_openai-1.3.6/serverless_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.5/setup.py` & `serverless_openai-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.5'
+VERSION = '1.3.6'
 DESCRIPTION = "A package for using Openai in serverless environment"
 LONG_DESCRIPTION = 'A package for using Openai with scraping and etc. in serverless application such as AWS Lambda and GCP Cloud Function'
 
 # Setting up
 setup(
     name="serverless_openai",
     version=VERSION,
```

