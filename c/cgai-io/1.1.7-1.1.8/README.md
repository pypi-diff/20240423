# Comparing `tmp/cgai_io-1.1.7.tar.gz` & `tmp/cgai_io-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgai_io-1.1.7.tar", last modified: Tue Jan 16 07:30:40 2024, max compression
+gzip compressed data, was "cgai_io-1.1.8.tar", last modified: Tue Apr 23 01:22:26 2024, max compression
```

## Comparing `cgai_io-1.1.7.tar` & `cgai_io-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 07:30:40.892405 cgai_io-1.1.7/
--rw-rw-rw-   0        0        0    35823 2024-01-16 07:22:37.000000 cgai_io-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     3792 2024-01-16 07:30:40.889542 cgai_io-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2967 2024-01-16 07:21:34.000000 cgai_io-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-16 07:30:40.874479 cgai_io-1.1.7/cgai_io/
--rw-rw-rw-   0        0        0     2912 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/Copy.py
--rw-rw-rw-   0        0        0     2606 2024-01-16 07:23:23.000000 cgai_io-1.1.7/cgai_io/Delete.py
--rw-rw-rw-   0        0        0      319 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/Info.py
--rw-rw-rw-   0        0        0      847 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/Move.py
--rw-rw-rw-   0        0        0      910 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/Name.py
--rw-rw-rw-   0        0        0      777 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/Pack.py
--rw-rw-rw-   0        0        0      408 2024-01-16 07:23:38.000000 cgai_io-1.1.7/cgai_io/__init__.py
--rw-rw-rw-   0        0        0      384 2024-01-16 07:21:34.000000 cgai_io-1.1.7/cgai_io/_util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 07:30:40.889542 cgai_io-1.1.7/cgai_io.egg-info/
--rw-rw-rw-   0        0        0     3792 2024-01-16 07:30:40.000000 cgai_io-1.1.7/cgai_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-01-16 07:30:40.000000 cgai_io-1.1.7/cgai_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 07:30:40.000000 cgai_io-1.1.7/cgai_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-01-16 07:30:40.000000 cgai_io-1.1.7/cgai_io.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-16 07:30:40.892909 cgai_io-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1166 2024-01-16 07:23:45.000000 cgai_io-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.819719 cgai_io-1.1.8/
+-rw-rw-rw-   0        0        0    35823 2024-04-23 01:15:31.000000 cgai_io-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3831 2024-04-23 01:22:26.818721 cgai_io-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2967 2024-04-23 01:15:31.000000 cgai_io-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.816728 cgai_io-1.1.8/cgai_io/
+-rw-rw-rw-   0        0        0     2912 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Copy.py
+-rw-rw-rw-   0        0        0     2606 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Delete.py
+-rw-rw-rw-   0        0        0      319 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Info.py
+-rw-rw-rw-   0        0        0      923 2024-04-23 01:12:13.000000 cgai_io-1.1.8/cgai_io/Move.py
+-rw-rw-rw-   0        0        0      910 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Name.py
+-rw-rw-rw-   0        0        0      777 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/Pack.py
+-rw-rw-rw-   0        0        0      408 2024-04-23 01:12:19.000000 cgai_io-1.1.8/cgai_io/__init__.py
+-rw-rw-rw-   0        0        0      384 2024-04-10 06:36:34.000000 cgai_io-1.1.8/cgai_io/_util.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:22:26.818721 cgai_io-1.1.8/cgai_io.egg-info/
+-rw-rw-rw-   0        0        0     3831 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 01:22:26.000000 cgai_io-1.1.8/cgai_io.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 01:22:26.819719 cgai_io-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2024-04-23 01:11:09.000000 cgai_io-1.1.8/setup.py
```

### Comparing `cgai_io-1.1.7/LICENSE` & `cgai_io-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/PKG-INFO` & `cgai_io-1.1.8/cgai_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: cgai_io
-Version: 1.1.7
+Name: cgai-io
+Version: 1.1.8
 Summary: A simple, light and fast data stream operation Python Library.
 Home-page: https://github.com/zxzxde/cgai-io
 Author: Master Zhang
 Author-email: 360014296@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -170,7 +172,8 @@
 # src_zip = r'D:\Temp\A\BB.zip'
 # des_dir = r'D:\Temp\A\C'
 # ci.unpack(src_zip,des_dir)
 ```
 
 #### 交流方式
 WeChat : zxzxde / 360014296
+
```

### Comparing `cgai_io-1.1.7/README.md` & `cgai_io-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/cgai_io/Copy.py` & `cgai_io-1.1.8/cgai_io/Copy.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/cgai_io/Delete.py` & `cgai_io-1.1.8/cgai_io/Delete.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/cgai_io/Name.py` & `cgai_io-1.1.8/cgai_io/Name.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/cgai_io/Pack.py` & `cgai_io-1.1.8/cgai_io/Pack.py`

 * *Files identical despite different names*

### Comparing `cgai_io-1.1.7/cgai_io.egg-info/PKG-INFO` & `cgai_io-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: cgai-io
-Version: 1.1.7
+Name: cgai_io
+Version: 1.1.8
 Summary: A simple, light and fast data stream operation Python Library.
 Home-page: https://github.com/zxzxde/cgai-io
 Author: Master Zhang
 Author-email: 360014296@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -170,7 +172,8 @@
 # src_zip = r'D:\Temp\A\BB.zip'
 # des_dir = r'D:\Temp\A\C'
 # ci.unpack(src_zip,des_dir)
 ```
 
 #### 交流方式
 WeChat : zxzxde / 360014296
+
```

### Comparing `cgai_io-1.1.7/setup.py` & `cgai_io-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cgai_io",
-    version="1.1.7",
+    version="1.1.8",
     author="Master Zhang",
     author_email="360014296@qq.com",
     description="A simple, light and fast data stream operation Python Library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zxzxde/cgai-io",
     packages=setuptools.find_packages(),
```

