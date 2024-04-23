# Comparing `tmp/usscore-0.0.6.tar.gz` & `tmp/usscore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/usscore-0.0.6.tar", last modified: Sun Mar 13 07:33:37 2022, max compression
+gzip compressed data, was "usscore-0.0.7.tar", last modified: Tue Apr 23 06:31:07 2024, max compression
```

## Comparing `usscore-0.0.6.tar` & `usscore-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-13 07:33:37.438679 usscore-0.0.6/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1913 2022-03-13 07:33:37.438679 usscore-0.0.6/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1378 2022-03-13 07:32:58.000000 usscore-0.0.6/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2022-03-13 07:33:37.438679 usscore-0.0.6/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      952 2022-03-13 07:29:18.000000 usscore-0.0.6/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-13 07:33:37.407424 usscore-0.0.6/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-13 07:33:37.438679 usscore-0.0.6/src/usscore.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1913 2022-03-13 07:33:36.000000 usscore-0.0.6/src/usscore.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2022-03-13 07:33:36.000000 usscore-0.0.6/src/usscore.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2022-03-13 07:33:36.000000 usscore-0.0.6/src/usscore.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2022-03-13 07:33:36.000000 usscore-0.0.6/src/usscore.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2022-03-13 07:33:36.000000 usscore-0.0.6/src/usscore.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1845 2022-03-13 07:29:01.000000 usscore-0.0.6/src/usscore.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-23 06:31:07.561813 usscore-0.0.7/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3401 2024-04-23 06:31:07.561813 usscore-0.0.7/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2861 2024-04-23 06:28:49.000000 usscore-0.0.7/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-23 06:31:07.561813 usscore-0.0.7/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      957 2024-04-23 06:28:03.000000 usscore-0.0.7/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-23 06:31:07.561813 usscore-0.0.7/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-23 06:31:07.561813 usscore-0.0.7/src/usscore.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3401 2024-04-23 06:31:07.000000 usscore-0.0.7/src/usscore.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-04-23 06:31:07.000000 usscore-0.0.7/src/usscore.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-23 06:31:07.000000 usscore-0.0.7/src/usscore.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-04-23 06:31:07.000000 usscore-0.0.7/src/usscore.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-04-23 06:31:07.000000 usscore-0.0.7/src/usscore.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1845 2022-03-13 07:29:01.000000 usscore-0.0.7/src/usscore.py
```

### Comparing `usscore-0.0.6/setup.py` & `usscore-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="usscore",
-    version="0.0.6",
+    version="0.0.7",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
-    description="A package for scoring state policies of covid-19 in the US",
+    description="PyPI package for scoring state policies of covid-19 in the US",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/scoreUS",
+    url="https://github.com/y-takefuji/scoreUS",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/scoreUS",
+        "Bug Tracker": "https://github.com/y-takefuji/scoreUS",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['usscore'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'usscore = usscore:main'
         ]
     },
 )
```

### Comparing `usscore-0.0.6/src/usscore.py` & `usscore-0.0.7/src/usscore.py`

 * *Files identical despite different names*

