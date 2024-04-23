# Comparing `tmp/jeffutils-0.4.9.tar.gz` & `tmp/jeffutils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.4.9.tar", last modified: Sat Apr 20 03:45:47 2024, max compression
+gzip compressed data, was "jeffutils-0.5.0.tar", last modified: Tue Apr 23 20:51:17 2024, max compression
```

## Comparing `jeffutils-0.4.9.tar` & `jeffutils-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.4.9/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-20 03:45:47.973482 jeffutils-0.4.9/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.4.9/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.4.9/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-20 03:45:47.973482 jeffutils-0.4.9/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-20 03:45:39.000000 jeffutils-0.4.9/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.4.9/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16086 2024-04-20 03:45:14.000000 jeffutils-0.4.9/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.0/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-23 20:51:17.689698 jeffutils-0.5.0/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.0/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.0/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-23 20:51:17.689698 jeffutils-0.5.0/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-23 20:51:12.000000 jeffutils-0.5.0/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.0/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16230 2024-04-23 20:50:46.000000 jeffutils-0.5.0/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-23 20:51:17.689698 jeffutils-0.5.0/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-23 20:51:17.000000 jeffutils-0.5.0/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.4.9/LICENSE.txt` & `jeffutils-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.4.9/setup.py` & `jeffutils-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.4.9',
+    version='0.5.0',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.4.9/src/jeffutils/utils.py` & `jeffutils-0.5.0/src/jeffutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
         with open(text_path, 'w+') as file:
             file.write(s.getvalue())
             
         if os.path.exists(prof_path):
             os.remove(prof_path)
 
             
-def print_skip_exceptions(full_stack_trace=True):
+def print_skip_exceptions(full_stack_trace=True, log_error=True):
     """ a decorator that will just print an exception thrown
     by the function without raising it up the call stack
     
     Ex:
     @print_skip_exceptions(True)
     def f():
         ...
@@ -442,17 +442,21 @@
                 result = func(*args, **kwargs)
                 return result
             except KeyboardInterrupt as e:
                 print("Caught KeyboardInterrupt and raising again")
                 raise e
             except Exception as e:
                 if full_stack_trace:
-                    print(stack_trace(e))
+                    string = stack_trace(e)
                 else:
-                    print(e)
+                    string = e
+                if log_error:
+                    log_print(string)
+                else:
+                    print(string)
                 return None
             
         return wrapper
     
     return wrap
```

