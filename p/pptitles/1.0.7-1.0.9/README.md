# Comparing `tmp/pptitles-1.0.7.tar.gz` & `tmp/pptitles-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptitles-1.0.7.tar", last modified: Tue Apr 23 20:13:24 2024, max compression
+gzip compressed data, was "pptitles-1.0.9.tar", last modified: Tue Apr 23 21:26:23 2024, max compression
```

## Comparing `pptitles-1.0.7.tar` & `pptitles-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:13:24.360233 pptitles-1.0.7/
--rw-r--r--   0 phx        (501) staff       (20)     1059 2024-04-23 19:47:35.000000 pptitles-1.0.7/LICENSE
--rw-r--r--   0 phx        (501) staff       (20)      614 2024-04-23 20:13:24.359779 pptitles-1.0.7/PKG-INFO
--rw-r--r--   0 phx        (501) staff       (20)      202 2024-04-23 20:11:05.000000 pptitles-1.0.7/README.md
--rwxr-xr-x   0 phx        (501) staff       (20)     2007 2024-04-23 19:44:05.000000 pptitles-1.0.7/pptitles
-drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 20:13:24.359364 pptitles-1.0.7/pptitles.egg-info/
--rw-r--r--   0 phx        (501) staff       (20)      614 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/PKG-INFO
--rw-r--r--   0 phx        (501) staff       (20)      163 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/SOURCES.txt
--rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/dependency_links.txt
--rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 20:13:24.000000 pptitles-1.0.7/pptitles.egg-info/top_level.txt
--rw-r--r--   0 phx        (501) staff       (20)       38 2024-04-23 20:13:24.360320 pptitles-1.0.7/setup.cfg
--rw-r--r--   0 phx        (501) staff       (20)      785 2024-04-23 20:13:19.000000 pptitles-1.0.7/setup.py
+drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 21:26:23.532798 pptitles-1.0.9/
+-rw-r--r--   0 phx        (501) staff       (20)     1059 2024-04-23 19:47:35.000000 pptitles-1.0.9/LICENSE
+-rw-r--r--   0 phx        (501) staff       (20)      641 2024-04-23 21:26:23.532382 pptitles-1.0.9/PKG-INFO
+-rw-r--r--   0 phx        (501) staff       (20)      202 2024-04-23 20:11:05.000000 pptitles-1.0.9/README.md
+-rwxr-xr-x   0 phx        (501) staff       (20)     2136 2024-04-23 21:16:12.000000 pptitles-1.0.9/pptitles
+drwxr-xr-x   0 phx        (501) staff       (20)        0 2024-04-23 21:26:23.531945 pptitles-1.0.9/pptitles.egg-info/
+-rw-r--r--   0 phx        (501) staff       (20)      641 2024-04-23 21:26:23.000000 pptitles-1.0.9/pptitles.egg-info/PKG-INFO
+-rw-r--r--   0 phx        (501) staff       (20)      194 2024-04-23 21:26:23.000000 pptitles-1.0.9/pptitles.egg-info/SOURCES.txt
+-rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 21:26:23.000000 pptitles-1.0.9/pptitles.egg-info/dependency_links.txt
+-rw-r--r--   0 phx        (501) staff       (20)       12 2024-04-23 21:26:23.000000 pptitles-1.0.9/pptitles.egg-info/requires.txt
+-rw-r--r--   0 phx        (501) staff       (20)        1 2024-04-23 21:26:23.000000 pptitles-1.0.9/pptitles.egg-info/top_level.txt
+-rw-r--r--   0 phx        (501) staff       (20)       38 2024-04-23 21:26:23.532886 pptitles-1.0.9/setup.cfg
+-rw-r--r--   0 phx        (501) staff       (20)      822 2024-04-23 21:26:17.000000 pptitles-1.0.9/setup.py
```

### Comparing `pptitles-1.0.7/LICENSE` & `pptitles-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pptitles-1.0.7/PKG-INFO` & `pptitles-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pptitles
-Version: 1.0.7
+Version: 1.0.9
 Summary: Extract the slide number and title from all slides in a PowerPoint presentation.
 Home-page: https://github.com/phx/pptitles
 Author: phx
 Author-email: phx@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-pptx
 
 # pptitles
 
 Extract the slide number and title from all slides in a PowerPoint presentation.
 
 ## Install from PyPi
```

### Comparing `pptitles-1.0.7/pptitles` & `pptitles-1.0.9/pptitles`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+
+import argparse
 import sys
 import re
 from pptx import Presentation
 
 def extract_titles(ppt_path):
     presentation = Presentation(ppt_path)
     titles = []
@@ -46,15 +48,15 @@
 
         title = best_candidate if best_candidate else "No title found"
         titles.append((i + 1, title))
 
     return titles
 
 if __name__ == "__main__":
-    if len(sys.argv) < 2:
-        print("Usage: python script.py 'path_to_presentation.pptx'")
-        sys.exit(1)
-    ppt_path = sys.argv[1]
+    parser = argparse.ArgumentParser(description="Process a PowerPoint file.")
+    parser.add_argument('-f', '--file', required=True, help="The filename of the PowerPoint presentation to process.")
+    args = parser.parse_args()
+    ppt_path = args.file
     titles = extract_titles(ppt_path)
     for slide_number, title in titles:
         print(f"Slide {slide_number}: {title}")
```

### Comparing `pptitles-1.0.7/pptitles.egg-info/PKG-INFO` & `pptitles-1.0.9/pptitles.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pptitles
-Version: 1.0.7
+Version: 1.0.9
 Summary: Extract the slide number and title from all slides in a PowerPoint presentation.
 Home-page: https://github.com/phx/pptitles
 Author: phx
 Author-email: phx@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-pptx
 
 # pptitles
 
 Extract the slide number and title from all slides in a PowerPoint presentation.
 
 ## Install from PyPi
```

### Comparing `pptitles-1.0.7/setup.py` & `pptitles-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pptitles',
-    version='1.0.7',
+    version='1.0.9',
     scripts=['pptitles'],  # Adjust as needed if it's a file or use glob.glob() for multiple files
     author='phx',
     author_email='phx@example.com',
     description='Extract the slide number and title from all slides in a PowerPoint presentation.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/phx/pptitles',
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
     ],
     package_dir={"": "."},
     packages=setuptools.find_packages(where="."),
     python_requires=">=3.6",
+    install_requires=['python-pptx']
 )
```

