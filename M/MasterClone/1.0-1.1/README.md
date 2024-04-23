# Comparing `tmp/masterclone-1.0.tar.gz` & `tmp/masterclone-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\cai\Desktop\MasterClone\dist\.tmp-3pm99kfx\masterclone-1.0.tar", last modified: Tue Apr 23 18:13:58 2024, max compression
+gzip compressed data, was "C:\Users\cai\Desktop\MasterClone\dist\.tmp-0wwc6nkx\masterclone-1.1.tar", last modified: Tue Apr 23 18:18:01 2024, max compression
```

## Comparing `masterclone-1.0.tar` & `masterclone-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:13:58.512379 masterclone-1.0/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:13:58.496779 masterclone-1.0/MasterClone.egg-info/
--rw-rw-rw-   0        0        0      494 2024-04-23 18:13:57.000000 masterclone-1.0/MasterClone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-23 18:13:58.000000 masterclone-1.0/MasterClone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:13:58.000000 masterclone-1.0/MasterClone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-23 18:13:58.000000 masterclone-1.0/MasterClone.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:13:58.000000 masterclone-1.0/MasterClone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      494 2024-04-23 18:13:58.512379 masterclone-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 16:35:01.000000 masterclone-1.0/license.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 18:13:58.527979 masterclone-1.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-04-23 18:10:40.000000 masterclone-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:01.818677 masterclone-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:01.662677 masterclone-1.1/MasterClone.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-23 18:17:59.000000 masterclone-1.1/MasterClone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-23 18:18:01.000000 masterclone-1.1/MasterClone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:17:59.000000 masterclone-1.1/MasterClone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 18:17:59.000000 masterclone-1.1/MasterClone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:17:59.000000 masterclone-1.1/MasterClone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      441 2024-04-23 18:18:01.818677 masterclone-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 16:35:01.000000 masterclone-1.1/license.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:18:01.834277 masterclone-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      564 2024-04-23 18:17:36.000000 masterclone-1.1/setup.py
```

### Comparing `masterclone-1.0/setup.py` & `masterclone-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MasterClone",
-    version="1.0",
+    version="1.1",
     author="caique9014",
     author_email="oldtimesonz@gmail.com",
     description="A tool for cloning Git repositories",
     url="https://github.com/NpmMaster/MasterClone.git",
     packages=find_packages(),
-    install_requires=['setuptools', 'pyautogui', 'subprocess', 'typer'],  # Add any dependencies here
+    install_requires=['setuptools','typer'],  # Add any dependencies here
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

