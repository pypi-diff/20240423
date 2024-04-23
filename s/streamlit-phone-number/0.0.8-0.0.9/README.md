# Comparing `tmp/streamlit-phone-number-0.0.8.tar.gz` & `tmp/streamlit-phone-number-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-phone-number-0.0.8.tar", last modified: Tue Apr 23 07:42:56 2024, max compression
+gzip compressed data, was "streamlit-phone-number-0.0.9.tar", last modified: Tue Apr 23 07:44:49 2024, max compression
```

## Comparing `streamlit-phone-number-0.0.8.tar` & `streamlit-phone-number-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.279843 streamlit-phone-number-0.0.8/
--rw-r--r--   0 wfluo      (502) staff       (20)       56 2023-06-28 05:50:16.000000 streamlit-phone-number-0.0.8/MANIFEST.in
--rw-r--r--   0 wfluo      (502) staff       (20)      957 2024-04-23 07:42:56.279602 streamlit-phone-number-0.0.8/PKG-INFO
--rw-r--r--   0 wfluo      (502) staff       (20)      303 2024-04-23 07:42:41.000000 streamlit-phone-number-0.0.8/README.md
--rw-r--r--   0 wfluo      (502) staff       (20)       38 2024-04-23 07:42:56.279905 streamlit-phone-number-0.0.8/setup.cfg
--rw-r--r--   0 wfluo      (502) staff       (20)      864 2023-06-28 06:34:48.000000 streamlit-phone-number-0.0.8/setup.py
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.273637 streamlit-phone-number-0.0.8/streamlit_phone_number/
--rw-r--r--   0 wfluo      (502) staff       (20)      951 2024-04-23 07:37:59.000000 streamlit-phone-number-0.0.8/streamlit_phone_number/__init__.py
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.272276 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.276823 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.279186 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/assets/
--rw-r--r--   0 wfluo      (502) staff       (20)   545007 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/assets/index-5136414f.js
--rw-r--r--   0 wfluo      (502) staff       (20)     4545 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/assets/index-9a42c5bf.css
--rw-r--r--   0 wfluo      (502) staff       (20)      460 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/index.html
--rw-r--r--   0 wfluo      (502) staff       (20)     1497 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/vite.svg
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:42:56.275838 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/
--rw-r--r--   0 wfluo      (502) staff       (20)      957 2024-04-23 07:42:56.000000 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/PKG-INFO
--rw-r--r--   0 wfluo      (502) staff       (20)      513 2024-04-23 07:42:56.000000 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/SOURCES.txt
--rw-r--r--   0 wfluo      (502) staff       (20)        1 2024-04-23 07:42:56.000000 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/dependency_links.txt
--rw-r--r--   0 wfluo      (502) staff       (20)       10 2024-04-23 07:42:56.000000 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/requires.txt
--rw-r--r--   0 wfluo      (502) staff       (20)       23 2024-04-23 07:42:56.000000 streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/top_level.txt
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.786369 streamlit-phone-number-0.0.9/
+-rw-r--r--   0 wfluo      (502) staff       (20)       56 2023-06-28 05:50:16.000000 streamlit-phone-number-0.0.9/MANIFEST.in
+-rw-r--r--   0 wfluo      (502) staff       (20)      957 2024-04-23 07:44:49.785999 streamlit-phone-number-0.0.9/PKG-INFO
+-rw-r--r--   0 wfluo      (502) staff       (20)      303 2024-04-23 07:42:41.000000 streamlit-phone-number-0.0.9/README.md
+-rw-r--r--   0 wfluo      (502) staff       (20)       38 2024-04-23 07:44:49.786460 streamlit-phone-number-0.0.9/setup.cfg
+-rw-r--r--   0 wfluo      (502) staff       (20)      864 2024-04-23 07:44:47.000000 streamlit-phone-number-0.0.9/setup.py
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.778783 streamlit-phone-number-0.0.9/streamlit_phone_number/
+-rw-r--r--   0 wfluo      (502) staff       (20)      951 2024-04-23 07:37:59.000000 streamlit-phone-number-0.0.9/streamlit_phone_number/__init__.py
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.777037 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.782368 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.785431 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/assets/
+-rw-r--r--   0 wfluo      (502) staff       (20)   545007 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/assets/index-5136414f.js
+-rw-r--r--   0 wfluo      (502) staff       (20)     4545 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/assets/index-9a42c5bf.css
+-rw-r--r--   0 wfluo      (502) staff       (20)      460 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/index.html
+-rw-r--r--   0 wfluo      (502) staff       (20)     1497 2024-04-23 07:35:37.000000 streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/vite.svg
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-23 07:44:49.781056 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/
+-rw-r--r--   0 wfluo      (502) staff       (20)      957 2024-04-23 07:44:49.000000 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/PKG-INFO
+-rw-r--r--   0 wfluo      (502) staff       (20)      513 2024-04-23 07:44:49.000000 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/SOURCES.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)        1 2024-04-23 07:44:49.000000 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/dependency_links.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)       10 2024-04-23 07:44:49.000000 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/requires.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)       23 2024-04-23 07:44:49.000000 streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/top_level.txt
```

### Comparing `streamlit-phone-number-0.0.8/PKG-INFO` & `streamlit-phone-number-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-phone-number
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/pragmatic-streamlit/streamlit-phone-number
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `streamlit-phone-number-0.0.8/setup.py` & `streamlit-phone-number-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-phone-number',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     include_package_data=True,
     install_requires=['streamlit'],
     url='https://github.com/pragmatic-streamlit/streamlit-phone-number',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number/__init__.py` & `streamlit-phone-number-0.0.9/streamlit_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/assets/index-5136414f.js` & `streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/assets/index-5136414f.js`

 * *Files identical despite different names*

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/assets/index-9a42c5bf.css` & `streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/assets/index-9a42c5bf.css`

 * *Files identical despite different names*

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number/frontend/dist/vite.svg` & `streamlit-phone-number-0.0.9/streamlit_phone_number/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/PKG-INFO` & `streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-phone-number
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/pragmatic-streamlit/streamlit-phone-number
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `streamlit-phone-number-0.0.8/streamlit_phone_number.egg-info/SOURCES.txt` & `streamlit-phone-number-0.0.9/streamlit_phone_number.egg-info/SOURCES.txt`

 * *Files identical despite different names*

