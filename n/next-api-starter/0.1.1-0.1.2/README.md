# Comparing `tmp/next-api-starter-0.1.1.tar.gz` & `tmp/next_api_starter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-api-starter-0.1.1.tar", last modified: Thu Apr 18 12:23:01 2024, max compression
+gzip compressed data, was "next_api_starter-0.1.2.tar", last modified: Tue Apr 23 07:23:38 2024, max compression
```

## Comparing `next-api-starter-0.1.1.tar` & `next_api_starter-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,30 @@
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-18 12:23:01.114781 next-api-starter-0.1.1/
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      219 2024-04-18 12:23:00.838788 next-api-starter-0.1.1/PKG-INFO
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-18 12:23:00.838788 next-api-starter-0.1.1/next_api_starter.egg-info/
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      219 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/PKG-INFO
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      250 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/SOURCES.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)        1 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/dependency_links.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)       71 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/entry_points.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)       18 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/requires.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)        1 2024-04-18 12:23:00.000000 next-api-starter-0.1.1/next_api_starter.egg-info/top_level.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)       38 2024-04-18 12:23:01.114781 next-api-starter-0.1.1/setup.cfg
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      768 2024-04-18 12:20:33.000000 next-api-starter-0.1.1/setup.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-18 19:15:04.000000 next_api_starter-0.1.2/LICENSE.txt
+-rw-r--r--   0 luffy     (1000) luffy     (1000)      223 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/PKG-INFO
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-18 19:15:04.000000 next_api_starter-0.1.2/README.md
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/next_api_starter.egg-info/
+-rw-r--r--   0 luffy     (1000) luffy     (1000)      223 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/PKG-INFO
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)      786 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/SOURCES.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        1 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/dependency_links.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       76 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/entry_points.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       18 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/requires.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        4 2024-04-23 07:23:37.000000 next_api_starter-0.1.2/next_api_starter.egg-info/top_level.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       38 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/setup.cfg
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)      734 2024-04-23 06:57:20.000000 next_api_starter-0.1.2/setup.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:37.967797 next_api_starter-0.1.2/src/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-18 19:18:29.000000 next_api_starter-0.1.2/src/__init__.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:37.983797 next_api_starter-0.1.2/src/next_api_starter/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-18 19:16:08.000000 next_api_starter-0.1.2/src/next_api_starter/__init__.py
+-rwxrwxr-x   0 luffy     (1000) luffy     (1000)     2219 2024-04-23 06:57:46.000000 next_api_starter-0.1.2/src/next_api_starter/create_nextapi.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       86 2024-04-18 19:16:28.000000 next_api_starter-0.1.2/src/next_api_starter/main.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:37.995797 next_api_starter-0.1.2/src/next_api_starter/template/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-22 18:44:19.000000 next_api_starter-0.1.2/src/next_api_starter/template/__init__.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/src/next_api_starter/template/backened/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:42:57.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/__init__.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:43:07.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/database.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:43:17.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/main.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:43:39.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/models.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2024-04-23 07:23:38.019797 next_api_starter-0.1.2/src/next_api_starter/template/backened/routers/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:49:11.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/routers/__init__.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:44:14.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/schemas.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        0 2024-04-19 08:44:32.000000 next_api_starter-0.1.2/src/next_api_starter/template/backened/utils.py
```

### Comparing `next-api-starter-0.1.1/setup.py` & `next_api_starter-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="next-api-starter",  # Replace with your desired package name
-    version="0.1.1",  # Start with version 0.1.0 for initial release
+    version="0.1.2",  # Start with version 0.1.0 for initial release
     description="Starter template for Next.js and FastAPI projects",
     long_description="...",  # Add detailed description in README format
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=["frontend", "backend", "tests"]),  # Exclude frontend/backend for separate installation
+    packages=find_packages(),  # Exclude frontend/backend for separate installation
     install_requires=[  # List dependencies for backend
         "uvicorn[standard]",
         # ... other dependencies
     ],
     entry_points={
         "console_scripts": [
-            "create_nextapi = create_nextapi.create_nextapi:main",
+            "create_nextapi = src.next_api_starter.create_nextapi:main",
         ]
     },
 )
```

