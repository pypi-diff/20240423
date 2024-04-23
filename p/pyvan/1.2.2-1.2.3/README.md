# Comparing `tmp/pyvan-1.2.2.tar.gz` & `tmp/pyvan-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvan-1.2.2.tar", last modified: Sun Dec 19 08:18:22 2021, max compression
+gzip compressed data, was "pyvan-1.2.3.tar", last modified: Tue Apr 23 06:07:59 2024, max compression
```

## Comparing `pyvan-1.2.2.tar` & `pyvan-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 acmt      (1000) acmt      (1000)        0 2021-12-19 08:18:22.694276 pyvan-1.2.2/
--rw-rw-r--   0 acmt      (1000) acmt      (1000)     5160 2021-12-19 08:18:22.690276 pyvan-1.2.2/PKG-INFO
--rw-rw-r--   0 acmt      (1000) acmt      (1000)     4065 2021-12-19 08:15:37.000000 pyvan-1.2.2/README.md
--rw-rw-r--   0 acmt      (1000) acmt      (1000)       38 2021-12-19 08:18:22.694276 pyvan-1.2.2/setup.cfg
--rw-rw-r--   0 acmt      (1000) acmt      (1000)      788 2021-12-19 08:18:18.000000 pyvan-1.2.2/setup.py
-drwxrwxr-x   0 acmt      (1000) acmt      (1000)        0 2021-12-19 08:18:22.686276 pyvan-1.2.2/src/
-drwxrwxr-x   0 acmt      (1000) acmt      (1000)        0 2021-12-19 08:18:22.690276 pyvan-1.2.2/src/pyvan.egg-info/
--rw-rw-r--   0 acmt      (1000) acmt      (1000)     5160 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/PKG-INFO
--rw-rw-r--   0 acmt      (1000) acmt      (1000)      231 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/SOURCES.txt
--rw-rw-r--   0 acmt      (1000) acmt      (1000)        1 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/dependency_links.txt
--rw-rw-r--   0 acmt      (1000) acmt      (1000)       37 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/entry_points.txt
--rw-rw-r--   0 acmt      (1000) acmt      (1000)       31 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/requires.txt
--rw-rw-r--   0 acmt      (1000) acmt      (1000)        6 2021-12-19 08:18:22.000000 pyvan-1.2.2/src/pyvan.egg-info/top_level.txt
--rw-rw-r--   0 acmt      (1000) acmt      (1000)    25146 2021-12-19 08:15:37.000000 pyvan-1.2.2/src/pyvan.py
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 06:07:59.590712 pyvan-1.2.3/
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     1070 2024-04-23 05:00:54.000000 pyvan-1.2.3/LICENSE
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     4387 2024-04-23 06:07:59.590712 pyvan-1.2.3/PKG-INFO
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     4184 2024-04-23 05:58:19.000000 pyvan-1.2.3/README.md
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       38 2024-04-23 06:07:59.590712 pyvan-1.2.3/setup.cfg
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)      787 2024-04-23 05:01:13.000000 pyvan-1.2.3/setup.py
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 06:07:59.590712 pyvan-1.2.3/src/
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 06:07:59.590712 pyvan-1.2.3/src/pyvan.egg-info/
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     4387 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/PKG-INFO
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)      239 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/SOURCES.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)        1 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/dependency_links.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       36 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/entry_points.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       31 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/requires.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)        6 2024-04-23 06:07:59.000000 pyvan-1.2.3/src/pyvan.egg-info/top_level.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)    28642 2024-04-23 06:01:08.000000 pyvan-1.2.3/src/pyvan.py
```

### Comparing `pyvan-1.2.2/README.md` & `pyvan-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 *Or*
 
 Make a "van.py" file next to the "main.py" file (entry point of your program) 
 
 Paste the code bellow:
 
-```py
+```python
+
 import pyvan
 
 OPTIONS = {
   "main_file_name": "main.py",
   "show_console": False,
   "use_existing_requirements": True,
   "extra_pip_install_args": [],
@@ -54,14 +55,15 @@
   "exclude_modules": [],
   "include_modules": [],
   "path_to_get_pip_and_python_embedded_zip": "",
   "build_dir": "dist",
   "pydist_sub_dir": "pydist",
   "source_sub_dir": "",
   "icon_file": None,
+  "verbose": True,
 }
 
 pyvan.build(**OPTIONS)
 
  
 ```
 
@@ -80,15 +82,16 @@
 exclude\_modules|[]|modules to exclude from bundle
 include\_modules|[]|modules to include in the bundle
 path\_to\_get\_pip\_and\_python\_embedded\_zip|''|by default is the Download path (path to 'get-pip.py' and 'python-x.x.x-embed-amdxx.zip' files)
 build\_dir|dist|the directory in which pyvan will create the stand-alone distribution
 pydist\_sub\_dir|pydist|a sub directory relative to `build_dir` where the stand-alone python distribution will be installed
 source\_sub\_dir|''|a sub directory relative to `build_dir` where the to execute python files will be installed
 input\_dir|'.'|the directory to get the main\_file\_name file from
-icon\_file|None|path to icon file to use for your application executable, doesn't use one by default 
+icon\_file|None|path to icon file to use for your application executable, doesn't use one by default
+verbose|True|Limit the amount of logs you see in the terminal. Show only warnings or errors.
 
 
 
 
 **Thanks to [silvandeleemput](https://github.com/silvandeleemput) for extending the available options, adding support for CLI commands, automating the download of get-pip.py, 
 embedded python zip and making possible the generation of an executable file!**
```

### Comparing `pyvan-1.2.2/setup.py` & `pyvan-1.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
-# python3 setup.py bdist_wheel sdist
+# python setup.py bdist_wheel sdist
 # cd dist
 # twine upload *
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pyvan",
-    version="1.2.2",
+    version="1.2.3",
     description="Make runnable desktop apps from your python scripts more easily with pyvan!",
     url="https://github.com/ClimenteA/pyvan",
     author="Climente Alin",
     author_email="climente.alin@gmail.com",
     license="MIT",
     py_modules=["pyvan"],
     install_requires=["pipreqs", "click", "requests", "gen-exe"],
```

