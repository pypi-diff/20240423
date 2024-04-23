# Comparing `tmp/crawlnet-0.0.1.tar.gz` & `tmp/crawlnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.1.tar", last modified: Tue Apr 23 10:49:44 2024, max compression
+gzip compressed data, was "crawlnet-0.0.2.tar", last modified: Tue Apr 23 12:58:54 2024, max compression
```

## Comparing `crawlnet-0.0.1.tar` & `crawlnet-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:49:44.266529 crawlnet-0.0.1/
--rw-rw-rw-   0        0        0      596 2024-04-23 10:49:44.264919 crawlnet-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-04-23 10:48:05.000000 crawlnet-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 10:49:44.219392 crawlnet-0.0.1/crawlnet/
--rw-rw-rw-   0        0        0       26 2024-04-23 10:46:52.000000 crawlnet-0.0.1/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    21578 2024-04-23 10:43:27.000000 crawlnet-0.0.1/crawlnet/cl3.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:49:44.262972 crawlnet-0.0.1/crawlnet.egg-info/
--rw-rw-rw-   0        0        0      596 2024-04-23 10:49:44.000000 crawlnet-0.0.1/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-23 10:49:44.000000 crawlnet-0.0.1/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:49:44.000000 crawlnet-0.0.1/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-23 10:49:44.000000 crawlnet-0.0.1/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 10:49:44.000000 crawlnet-0.0.1/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 10:49:44.267462 crawlnet-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-04-23 10:45:29.000000 crawlnet-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.991434 crawlnet-0.0.2/
+-rw-rw-rw-   0        0        0      794 2024-04-23 12:58:54.990189 crawlnet-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.964859 crawlnet-0.0.2/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.2/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    21578 2024-04-23 10:43:27.000000 crawlnet-0.0.2/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.2/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.989179 crawlnet-0.0.2/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0      794 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:58:54.991434 crawlnet-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-23 12:56:04.000000 crawlnet-0.0.2/setup.py
```

### Comparing `crawlnet-0.0.1/crawlnet/cl3.py` & `crawlnet-0.0.2/crawlnet/cl3.py`

 * *Files identical despite different names*

### Comparing `crawlnet-0.0.1/setup.py` & `crawlnet-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
-DESCRIPTION = 'CrawlNet'
- 
+VERSION = "0.0.2"
+DESCRIPTION = "CrawlNet"
+
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
     author_email="<hrushiskachgunde@gmail.com>",
     description=DESCRIPTION,
-    long_description=open('README.md').read(),
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=['numpy', 'matplotlib', "deap", "pandas"],
-    keywords=['python'],
+    install_requires=["numpy", "matplotlib", "deap", "pandas"],
+    keywords=["python"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
-)
+    ],
+)
```

