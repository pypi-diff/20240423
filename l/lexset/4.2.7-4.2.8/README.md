# Comparing `tmp/lexset-4.2.7.tar.gz` & `tmp/lexset-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.2.7.tar", last modified: Thu Dec 21 00:09:10 2023, max compression
+gzip compressed data, was "lexset-4.2.8.tar", last modified: Tue Apr 23 21:57:59 2024, max compression
```

## Comparing `lexset-4.2.7.tar` & `lexset-4.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 00:09:10.427785 lexset-4.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-21 00:09:10.427785 lexset-4.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-21 00:08:50.000000 lexset-4.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 00:09:10.427785 lexset-4.2.7/lexset/
--rw-r--r--   0 runner    (1001) docker     (127)    28493 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/medtronic_Debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/review.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-12-21 00:08:50.000000 lexset-4.2.7/lexset/test_ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 00:09:10.427785 lexset-4.2.7/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-21 00:09:10.000000 lexset-4.2.7/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-21 00:09:10.000000 lexset-4.2.7/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 00:09:10.000000 lexset-4.2.7/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-21 00:09:10.000000 lexset-4.2.7/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-21 00:09:10.000000 lexset-4.2.7/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 00:09:10.427785 lexset-4.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-21 00:08:50.000000 lexset-4.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 21:57:59.898743 lexset-4.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 21:57:49.000000 lexset-4.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/lexset/
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/medtronic_Debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/test_ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:57:59.898743 lexset-4.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-23 21:57:49.000000 lexset-4.2.8/setup.py
```

### Comparing `lexset-4.2.7/lexset/LexsetManager.py` & `lexset-4.2.8/lexset/LexsetManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         def delete_bin_files(parts):
             for i in range(parts):
                 os.remove(f"part{i}.bin")
 
         #function that downloads a part of the file and saves it to disk
         def download_part(start, end, part_number, progress_bar):
             headers = {"Authorization": f"Bearer {bearer_token}", "Range": f"bytes={start}-{end}"}
-            response = requests.get(url, headers=headers, stream=True)
+            response = requests.get(url, headers=headers, stream=True, verify=False)
 
             with open(f"part{part_number}.bin", "wb") as f:
                 for chunk in response.iter_content(chunk_size=1024*1024):
                     f.write(chunk)
                     progress_bar.update(len(chunk))
 
         if self.complete == True:
@@ -259,15 +259,15 @@
         for id in id_list:
             url = "https://coreapi.lexset.ai/api/dataset/download/" + str(id) + "/dataset.zip"
             bearer_token = self.token
             
             headers = {"Authorization": f"Bearer {bearer_token}"}
 
             session = requests.Session()
-            response = session.get(url, headers=headers, stream=True)
+            response = session.get(url, headers=headers, stream=True, verify=False)
                 
             #MAKE REQUEST TO GET THE FILE SIZE FROM THE HEADERS note: we could possibly remove this if we chane the server side code.
             if response.status_code == 401:
                 print("\33[1;31;40mUnauthorized: " + str(response.status_code) + "\33[0m")
                 return("Unauthorized")
             if response.status_code == 500:
                 print("\33[1;31;40mdownload() Error: " + str(response.status_code) + " please contact support." +"\33[0m")
```

### Comparing `lexset-4.2.7/lexset/credentials.py` & `lexset-4.2.8/lexset/credentials.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.7/lexset/medtronic_Debug.py` & `lexset-4.2.8/lexset/medtronic_Debug.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.7/lexset/review.py` & `lexset-4.2.8/lexset/review.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.7/lexset/test_ssim.py` & `lexset-4.2.8/lexset/test_ssim.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.7/setup.py` & `lexset-4.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='lexset',
-      version='4.2.7',
+      version='4.2.8',
       author='F. Bitonti',
       author_email='Francis@lexset.ai',
       license='Apache 2.0',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3'
       ],
```

