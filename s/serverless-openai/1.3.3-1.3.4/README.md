# Comparing `tmp/serverless_openai-1.3.3.tar.gz` & `tmp/serverless_openai-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless_openai-1.3.3.tar", last modified: Thu Feb 22 00:48:26 2024, max compression
+gzip compressed data, was "serverless_openai-1.3.4.tar", last modified: Tue Apr 23 10:14:41 2024, max compression
```

## Comparing `serverless_openai-1.3.3.tar` & `serverless_openai-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:48:26.535184 serverless_openai-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-22 00:48:26.535184 serverless_openai-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 00:48:16.000000 serverless_openai-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:48:26.535184 serverless_openai-1.3.3/serverless_openai/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 00:48:16.000000 serverless_openai-1.3.3/serverless_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-02-22 00:48:16.000000 serverless_openai-1.3.3/serverless_openai/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-02-22 00:48:16.000000 serverless_openai-1.3.3/serverless_openai/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:48:26.535184 serverless_openai-1.3.3/serverless_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-22 00:48:26.000000 serverless_openai-1.3.3/serverless_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-22 00:48:26.000000 serverless_openai-1.3.3/serverless_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 00:48:26.000000 serverless_openai-1.3.3/serverless_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 00:48:26.000000 serverless_openai-1.3.3/serverless_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 00:48:26.000000 serverless_openai-1.3.3/serverless_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 00:48:26.535184 serverless_openai-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-22 00:48:16.000000 serverless_openai-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/serverless_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/serverless_openai/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/serverless_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 10:14:41.000000 serverless_openai-1.3.4/serverless_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:14:41.295182 serverless_openai-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 10:14:37.000000 serverless_openai-1.3.4/setup.py
```

### Comparing `serverless_openai-1.3.3/PKG-INFO` & `serverless_openai-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.3
+Version: 1.3.4
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.3/serverless_openai/apis.py` & `serverless_openai-1.3.4/serverless_openai/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,23 +234,34 @@
             messages: VisionMessage,
             model: Union[VisionModels, str] = VisionModels.gpt4_vision,
             tries: int = 5,
             timeout: int = 500,
             temperature: Optional[float] = 1,
             max_tokens: Optional[int] = 1024,
         ) -> OpenAIResults:
+        
+        if isinstance(messages.image, list):
+            img_b64_list = []
+            for img in messages.image:
+                if 'data:image/jpeg;base64' in img:
+                    image_np = b64_to_np(img)
+                else:
+                    image_np = urlimage_to_np(img)
+                img_b64_list.extend(crop_image(image_np))
 
-        if isinstance(messages.image, str):
+        elif isinstance(messages.image, str):
             if 'data:image/jpeg;base64' in messages.image:
                 image_np = b64_to_np(messages.image)
             else:
                 image_np = urlimage_to_np(messages.image)
+            img_b64_list = crop_image(image_np)
         elif isinstance(messages.image, np.ndarray):
             image_np = messages.image
-        img_b64_list = crop_image(image_np)
+            img_b64_list = crop_image(image_np)
+            
         newm = [
             {
                 "role": messages.role,
                 "content": [
                     {
                         "type": "text",
                         "text": messages.text
```

### Comparing `serverless_openai-1.3.3/serverless_openai/helpers.py` & `serverless_openai-1.3.4/serverless_openai/helpers.py`

 * *Files identical despite different names*

### Comparing `serverless_openai-1.3.3/serverless_openai.egg-info/PKG-INFO` & `serverless_openai-1.3.4/serverless_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.3
+Version: 1.3.4
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.3/setup.py` & `serverless_openai-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.3'
+VERSION = '1.3.4'
 DESCRIPTION = "A package for using Openai in serverless environment"
 LONG_DESCRIPTION = 'A package for using Openai with scraping and etc. in serverless application such as AWS Lambda and GCP Cloud Function'
 
 # Setting up
 setup(
     name="serverless_openai",
     version=VERSION,
```

