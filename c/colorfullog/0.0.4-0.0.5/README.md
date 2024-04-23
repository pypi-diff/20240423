# Comparing `tmp/colorfullog-0.0.4.tar.gz` & `tmp/colorfullog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorfullog-0.0.4.tar", last modified: Tue Apr 23 03:11:56 2024, max compression
+gzip compressed data, was "colorfullog-0.0.5.tar", last modified: Tue Apr 23 04:46:52 2024, max compression
```

## Comparing `colorfullog-0.0.4.tar` & `colorfullog-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 03:11:56.952018 colorfullog-0.0.4/
--rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-23 03:11:56.952018 colorfullog-0.0.4/PKG-INFO
--rw-r--r--   0 ares      (1000) ares      (1000)      518 2024-04-17 06:47:59.000000 colorfullog-0.0.4/README.md
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 03:11:56.952018 colorfullog-0.0.4/colorfullog/
--rw-r--r--   0 ares      (1000) ares      (1000)       90 2024-04-17 07:14:01.000000 colorfullog-0.0.4/colorfullog/__init__.py
--rw-r--r--   0 ares      (1000) ares      (1000)     3245 2018-06-21 03:15:57.000000 colorfullog-0.0.4/colorfullog/colorfullog.py
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 03:11:56.952018 colorfullog-0.0.4/colorfullog/libs/
--rw-rw-r--   0 ares      (1000) ares      (1000)        0 2024-04-17 07:03:38.000000 colorfullog-0.0.4/colorfullog/libs/__init__.py
--rw-------   0 ares      (1000) ares      (1000)    96311 2022-07-15 03:49:46.000000 colorfullog-0.0.4/colorfullog/libs/argparse.py
--rw-------   0 ares      (1000) ares      (1000)    41477 2024-04-17 07:01:46.000000 colorfullog-0.0.4/colorfullog/libs/os.py
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 03:11:56.952018 colorfullog-0.0.4/colorfullog.egg-info/
--rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-23 03:11:56.000000 colorfullog-0.0.4/colorfullog.egg-info/PKG-INFO
--rw-rw-r--   0 ares      (1000) ares      (1000)      300 2024-04-23 03:11:56.000000 colorfullog-0.0.4/colorfullog.egg-info/SOURCES.txt
--rw-rw-r--   0 ares      (1000) ares      (1000)        1 2024-04-23 03:11:56.000000 colorfullog-0.0.4/colorfullog.egg-info/dependency_links.txt
--rw-rw-r--   0 ares      (1000) ares      (1000)       12 2024-04-23 03:11:56.000000 colorfullog-0.0.4/colorfullog.egg-info/top_level.txt
--rw-r--r--   0 ares      (1000) ares      (1000)       38 2024-04-23 03:11:56.952018 colorfullog-0.0.4/setup.cfg
--rw-r--r--   0 ares      (1000) ares      (1000)     1315 2024-04-23 03:07:28.000000 colorfullog-0.0.4/setup.py
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 04:46:52.726432 colorfullog-0.0.5/
+-rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-23 04:46:52.730432 colorfullog-0.0.5/PKG-INFO
+-rw-r--r--   0 ares      (1000) ares      (1000)      518 2024-04-17 06:47:59.000000 colorfullog-0.0.5/README.md
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 04:46:52.726432 colorfullog-0.0.5/colorfullog/
+-rw-r--r--   0 ares      (1000) ares      (1000)       69 2024-04-23 04:46:04.000000 colorfullog-0.0.5/colorfullog/__init__.py
+-rw-r--r--   0 ares      (1000) ares      (1000)     3245 2018-06-21 03:15:57.000000 colorfullog-0.0.5/colorfullog/colorfullog.py
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-23 04:46:52.726432 colorfullog-0.0.5/colorfullog.egg-info/
+-rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-23 04:46:52.000000 colorfullog-0.0.5/colorfullog.egg-info/PKG-INFO
+-rw-rw-r--   0 ares      (1000) ares      (1000)      219 2024-04-23 04:46:52.000000 colorfullog-0.0.5/colorfullog.egg-info/SOURCES.txt
+-rw-rw-r--   0 ares      (1000) ares      (1000)        1 2024-04-23 04:46:52.000000 colorfullog-0.0.5/colorfullog.egg-info/dependency_links.txt
+-rw-rw-r--   0 ares      (1000) ares      (1000)       12 2024-04-23 04:46:52.000000 colorfullog-0.0.5/colorfullog.egg-info/top_level.txt
+-rw-r--r--   0 ares      (1000) ares      (1000)       38 2024-04-23 04:46:52.730432 colorfullog-0.0.5/setup.cfg
+-rw-r--r--   0 ares      (1000) ares      (1000)     1315 2024-04-23 04:46:23.000000 colorfullog-0.0.5/setup.py
```

### Comparing `colorfullog-0.0.4/README.md` & `colorfullog-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `colorfullog-0.0.4/colorfullog/colorfullog.py` & `colorfullog-0.0.5/colorfullog/colorfullog.py`

 * *Files identical despite different names*

### Comparing `colorfullog-0.0.4/setup.py` & `colorfullog-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 long_description = 'set console color of font'
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setuptools.setup(
     name="colorfullog",
-    version="0.0.4",
+    version="0.0.5",
     author="Peng Shiyu",
     license = 'MIT License',
     author_email="pengshiyuyx@gmail.com",
     description="set console color of font",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/mouday/colorfullog",
```

