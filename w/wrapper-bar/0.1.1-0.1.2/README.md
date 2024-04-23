# Comparing `tmp/wrapper_bar-0.1.1.tar.gz` & `tmp/wrapper_bar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapper_bar-0.1.1.tar", last modified: Tue Apr 23 03:28:57 2024, max compression
+gzip compressed data, was "wrapper_bar-0.1.2.tar", last modified: Tue Apr 23 04:18:58 2024, max compression
```

## Comparing `wrapper_bar-0.1.1.tar` & `wrapper_bar-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 03:28:57.257304 wrapper_bar-0.1.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-22 04:51:36.000000 wrapper_bar-0.1.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4085 2024-04-23 03:28:57.256977 wrapper_bar-0.1.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1756 2024-04-23 03:27:06.000000 wrapper_bar-0.1.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1210 2024-04-22 19:10:38.000000 wrapper_bar-0.1.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-23 03:28:57.257365 wrapper_bar-0.1.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 03:28:57.250675 wrapper_bar-0.1.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 03:28:57.253463 wrapper_bar-0.1.1/src/wrapper_bar/
--rw-r--r--   0 d33pster   (501) staff       (20)       24 2024-04-22 20:39:35.000000 wrapper_bar-0.1.1/src/wrapper_bar/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     6491 2024-04-22 20:57:14.000000 wrapper_bar-0.1.1/src/wrapper_bar/wrapper.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 03:28:57.256653 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4085 2024-04-23 03:28:57.000000 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      281 2024-04-23 03:28:57.000000 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-23 03:28:57.000000 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       21 2024-04-23 03:28:57.000000 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       12 2024-04-23 03:28:57.000000 wrapper_bar-0.1.1/src/wrapper_bar.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 04:18:58.284736 wrapper_bar-0.1.2/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-22 04:51:36.000000 wrapper_bar-0.1.2/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4283 2024-04-23 04:18:58.284400 wrapper_bar-0.1.2/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1954 2024-04-23 04:18:20.000000 wrapper_bar-0.1.2/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1210 2024-04-23 03:54:32.000000 wrapper_bar-0.1.2/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-23 04:18:58.284792 wrapper_bar-0.1.2/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 04:18:58.278579 wrapper_bar-0.1.2/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 04:18:58.280115 wrapper_bar-0.1.2/src/wrapper_bar/
+-rw-r--r--   0 d33pster   (501) staff       (20)       24 2024-04-22 20:39:35.000000 wrapper_bar-0.1.2/src/wrapper_bar/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7532 2024-04-23 04:15:57.000000 wrapper_bar-0.1.2/src/wrapper_bar/wrapper.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 04:18:58.283990 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4283 2024-04-23 04:18:58.000000 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      281 2024-04-23 04:18:58.000000 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-23 04:18:58.000000 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       21 2024-04-23 04:18:58.000000 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       12 2024-04-23 04:18:58.000000 wrapper_bar-0.1.2/src/wrapper_bar.egg-info/top_level.txt
```

### Comparing `wrapper_bar-0.1.1/LICENSE` & `wrapper_bar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapper_bar-0.1.1/PKG-INFO` & `wrapper_bar-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapper-bar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Progress Bar with command wrapping
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -64,15 +64,15 @@
 - [Uninstall](#uninstall)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.1
+pip install wrapper-bar==0.1.2
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -110,14 +110,21 @@
 
   - `pyWrapper`
 
     ```python
     >>> wrapControl.pyWrapper(*params) # parameters are in the docstring.
     # pyWrapper can wrap list of python scripts across the progressbar.
     ```
+  
+  - `pyShellWrapper`
+  
+    ```python
+    >>> wrapControl.pyShellWrapper(*params) # parametes are in the docstring.
+    # pyShellWrapper can wrap inline python code across a progressbar.
+    ```
 
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
```

### Comparing `wrapper_bar-0.1.1/README.md` & `wrapper_bar-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - [Uninstall](#uninstall)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.1
+pip install wrapper-bar==0.1.2
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -63,14 +63,21 @@
 
   - `pyWrapper`
 
     ```python
     >>> wrapControl.pyWrapper(*params) # parameters are in the docstring.
     # pyWrapper can wrap list of python scripts across the progressbar.
     ```
+  
+  - `pyShellWrapper`
+  
+    ```python
+    >>> wrapControl.pyShellWrapper(*params) # parametes are in the docstring.
+    # pyShellWrapper can wrap inline python code across a progressbar.
+    ```
 
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
```

### Comparing `wrapper_bar-0.1.1/pyproject.toml` & `wrapper_bar-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wrapper-bar"
-version = "0.1.1"
+version = "0.1.2"
 description = "Progress Bar with command wrapping"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wrapper_bar-0.1.1/src/wrapper_bar/wrapper.py` & `wrapper_bar-0.1.2/src/wrapper_bar/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     
     >>> wrapControl = Wrapper(label="Loading:")
     >>> wrapControl.decoy() # for demonstration.
     
     `Other Functions include:`
     >>> wrapControl.shellWrapper(<params>) # wrap shell commands into a progress bar.
     >>> wrapControl.pyWrapper(<params>) # wrap python scripts into a progress bar.
+    >>> wrapControl.pyShellWrapper(<params>) # wrap inline python codes into a progress bar.
     
     `Parameters:`
     # Wrapper class
     >>> wrapControl = Wrapper(label:str (optional), marker:str (optional))
     # decoy function
     >>> wrapControl.decoy(delay:float (optional), width:float (optional))
     # shellWrapper function
@@ -56,14 +57,17 @@
                                  logfile:TextIOWrapper (optional),
                                  logfile_auto_close:bool (optional))
     # pyWrapper function
     >>> wrapControl.pyWrapper(pythonscripts:list[str], delay:float (optional),
                                  width:float (optional), logger:bool (optional),
                                  logfile:TextIOWrapper (optional),
                                  logfile_auto_close:bool (optional))
+    # pyShellWrapper function
+    >>> wrapControl.pyShellWrapper(pythoncodes: list[str], delay:float (optional),
+                                   width:float (optional))
     
     For Beginners, wrapping commands across a given progress bar might seem
     awfully time consuming. This Module is an effort to provide satisfaction to
     your aesthetic needs for your scripts.
     
     Feel free to check out the code and do any modifications you like under the
     MIT License. ;)
@@ -141,8 +145,28 @@
             else:
                 sleep(delay)
                 bar.update(i)
         
         bar.finish()
         
         if logfile_auto_close:
-            logfile.close()
+            logfile.close()
+    
+    def pyShellWrapper(self, pythoncodes: list[str], delay:float = 0.1, width:float = 50):
+        """Wrap inline python codes with a progressbar"""
+        
+        widgets = [self.label+" ", progressbar.Bar(marker=self.marker), progressbar.AdaptiveETA()]
+        bar = progressbar.ProgressBar(widgets=widgets, maxval=100, term_width=width).start()
+        
+        interval = int(100/(len(pythoncodes)+1))
+        iterator = 0
+        
+        for i in range(100):
+            if i>=interval and (i==interval or i%interval==0) and iterator<len(pythoncodes):
+                exec(pythoncodes[iterator])
+                iterator += 1
+                bar.update(i)
+            else:
+                sleep(delay)
+                bar.update(i)
+        
+        bar.finish()
```

### Comparing `wrapper_bar-0.1.1/src/wrapper_bar.egg-info/PKG-INFO` & `wrapper_bar-0.1.2/src/wrapper_bar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapper-bar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Progress Bar with command wrapping
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -64,15 +64,15 @@
 - [Uninstall](#uninstall)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.1
+pip install wrapper-bar==0.1.2
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -110,14 +110,21 @@
 
   - `pyWrapper`
 
     ```python
     >>> wrapControl.pyWrapper(*params) # parameters are in the docstring.
     # pyWrapper can wrap list of python scripts across the progressbar.
     ```
+  
+  - `pyShellWrapper`
+  
+    ```python
+    >>> wrapControl.pyShellWrapper(*params) # parametes are in the docstring.
+    # pyShellWrapper can wrap inline python code across a progressbar.
+    ```
 
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
```

