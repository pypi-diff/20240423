# Comparing `tmp/bogrod-0.3.0.tar.gz` & `tmp/bogrod-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bogrod-0.3.0.tar", last modified: Fri Apr 21 11:47:49 2023, max compression
+gzip compressed data, was "bogrod-0.4.0.tar", last modified: Tue Apr 23 11:42:02 2024, max compression
```

## Comparing `bogrod-0.3.0.tar` & `bogrod-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-21 11:47:49.060946 bogrod-0.3.0/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1080 2023-01-20 14:08:43.000000 bogrod-0.3.0/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3008 2023-04-21 11:47:49.060946 bogrod-0.3.0/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2705 2023-04-21 11:29:57.000000 bogrod-0.3.0/README.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-21 11:47:49.056946 bogrod-0.3.0/bogrod/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10885 2023-04-20 18:27:50.000000 bogrod-0.3.0/bogrod/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-21 11:47:49.060946 bogrod-0.3.0/bogrod/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2022-12-22 20:02:45.000000 bogrod-0.3.0/bogrod/tests/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1222 2022-12-22 22:59:53.000000 bogrod-0.3.0/bogrod/tests/test_bogrod.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-21 11:47:49.056946 bogrod-0.3.0/bogrod.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3008 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      280 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       39 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       11 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-04-21 11:47:49.000000 bogrod-0.3.0/bogrod.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-21 11:47:49.060946 bogrod-0.3.0/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      721 2023-04-21 11:30:40.000000 bogrod-0.3.0/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1080 2024-03-12 07:50:14.000000 bogrod-0.4.0/LICENSE
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12143 2024-04-23 11:42:02.974526 bogrod-0.4.0/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11646 2024-03-12 07:50:15.000000 bogrod-0.4.0/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    36873 2024-04-08 19:35:52.000000 bogrod-0.4.0/bogrod/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3306 2024-04-08 19:31:09.000000 bogrod-0.4.0/bogrod/sbom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      110 2024-04-08 19:27:37.000000 bogrod-0.4.0/bogrod/settings.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2022-12-22 20:02:45.000000 bogrod-0.4.0/bogrod/tests/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1382 2024-04-08 19:35:02.000000 bogrod-0.4.0/bogrod/tests/test_bogrod.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2849 2024-04-08 19:35:02.000000 bogrod-0.4.0/bogrod/util.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      283 2024-04-08 19:31:09.000000 bogrod-0.4.0/bogrod/vexfile.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod.egg-info/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12143 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      347 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       39 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/entry_points.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       74 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2024-04-23 11:42:02.978525 bogrod-0.4.0/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      942 2024-04-08 19:35:02.000000 bogrod-0.4.0/setup.py
```

### Comparing `bogrod-0.3.0/LICENSE` & `bogrod-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bogrod-0.3.0/setup.py` & `bogrod-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,22 @@
     license='MIT',
     author='Patrick Senti',
     author_email='patrick@productaize.io',
     description='Manage SBOM, VEX records and release notes in a single tool',
     long_description=README,
     long_description_content_type='text/markdown',
     install_requires=[
-        'jsonschema',
+        'jsonschema<4', # 4.x causes endless loop when validating with bom-1.5.schema.json
+        'pyyaml',
+        'tabulate',
+        'attrdict',
+        'textual',
+        'textual-dev', # for testing
+        'requests',
+        'yaspin',
     ],
     entry_points = {
         'console_scripts': [
             'bogrod=bogrod:main'
         ]
     }
 )
```

