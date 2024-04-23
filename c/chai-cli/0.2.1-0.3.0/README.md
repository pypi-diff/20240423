# Comparing `tmp/chai-cli-0.2.1.tar.gz` & `tmp/chai_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chai-cli-0.2.1.tar", last modified: Wed Apr 10 20:06:27 2024, max compression
+gzip compressed data, was "chai_cli-0.3.0.tar", last modified: Tue Apr 23 13:48:59 2024, max compression
```

## Comparing `chai-cli-0.2.1.tar` & `chai_cli-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.792179 chai-cli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 20:06:24.000000 chai-cli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-10 20:06:27.788179 chai-cli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 20:06:24.000000 chai-cli-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:06:27.792179 chai-cli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 20:06:24.000000 chai-cli-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/chai/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-10 20:06:24.000000 chai-cli-0.2.1/src/chai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 20:06:24.000000 chai-cli-0.2.1/src/chai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/chai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:48:59.638278 chai_cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 13:48:50.000000 chai_cli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-23 13:48:59.638278 chai_cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-23 13:48:50.000000 chai_cli-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:48:59.638278 chai_cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 13:48:50.000000 chai_cli-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:48:59.634278 chai_cli-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:48:59.638278 chai_cli-0.3.0/src/chai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-23 13:48:50.000000 chai_cli-0.3.0/src/chai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 13:48:50.000000 chai_cli-0.3.0/src/chai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:48:59.638278 chai_cli-0.3.0/src/chai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 13:48:59.000000 chai_cli-0.3.0/src/chai_cli.egg-info/top_level.txt
```

### Comparing `chai-cli-0.2.1/LICENSE` & `chai_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chai-cli-0.2.1/PKG-INFO` & `chai_cli-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: chai-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: AI in your CLI.
 Author: Ritik Sahni
 Author-email: ritiksahni0203@gmail.com
 Keywords: ai,openai,cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: argparse
+Requires-Dist: pyperclip
 
 # Chai - AI in your CLI.
 
 ## Introduction
 
 Chai is a command-line interface (CLI) tool designed to simplify your experience with bash commands. Have you ever found yourself stuck, not knowing the right bash command to use? With Chai, you can simply run `chai [your query in English]`, and it will respond with the appropriate bash command to help you out. 
 
@@ -41,14 +42,22 @@
 
 You can install Chai via pip:
 
 ```
 pip install chai-cli
 ```
 
+### Clipboard
+
+Every output is copied to your clipboard. To ensure that it works, run the following command to install required tools on Linux.
+
+```
+sudo apt-get install xclip xsel wl-clipboard
+```
+
 ## Examples
 
 Here are some examples of queries you can ask Chai:
 
 - "list all files starting with a"
 - "grep emails.txt for yahoo addresses"
 - "list users who are logged in"
```

### Comparing `chai-cli-0.2.1/README.md` & `chai_cli-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
 You can install Chai via pip:
 
 ```
 pip install chai-cli
 ```
 
+### Clipboard
+
+Every output is copied to your clipboard. To ensure that it works, run the following command to install required tools on Linux.
+
+```
+sudo apt-get install xclip xsel wl-clipboard
+```
+
 ## Examples
 
 Here are some examples of queries you can ask Chai:
 
 - "list all files starting with a"
 - "grep emails.txt for yahoo addresses"
 - "list users who are logged in"
```

### Comparing `chai-cli-0.2.1/setup.py` & `chai_cli-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='chai-cli',
-    version='0.2.1',
+    version='0.3.0',
     author='Ritik Sahni',
     author_email='ritiksahni0203@gmail.com',
     description='AI in your CLI.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['ai', 'openai', 'cli'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'openai',
-        'argparse'
+        'argparse',
+        'pyperclip'
     ],
     entry_points={
         'console_scripts': [
             'chai = chai:main',
         ]
     }
 )
```

### Comparing `chai-cli-0.2.1/src/chai/__init__.py` & `chai_cli-0.3.0/src/chai/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import argparse
 import os
 import sys
 import openai
+import pyperclip
 
 def main():
     if(os.environ.get('OPENAI_API_KEY') is None):
         sys.exit("Configure your OpenAI API Key. Export OPENAI_API_KEY environment variable your key to use Chai")
 
     parser = argparse.ArgumentParser(description='AI in your CLI')
     parser.add_argument('args', nargs='*', help="Query in natural language")
     args = parser.parse_args()
     response = queryGPT(args.args[0])
     print(response)
+    pyperclip.copy(response)
 
 
 def queryGPT(userQuery):
     if(userQuery is None):
         sys.exit()
 
     prompt = "You are an expert in using command-line interfaces. Every time I ask you a question or share my problem when I'm stuck in the command line, you must respond with a Linux command. You're only allowed to respond with a command to help when I'm stuck. No formatting, just the command that one can copy-and-paste in the terminal"
```

### Comparing `chai-cli-0.2.1/src/chai_cli.egg-info/PKG-INFO` & `chai_cli-0.3.0/src/chai_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: chai-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: AI in your CLI.
 Author: Ritik Sahni
 Author-email: ritiksahni0203@gmail.com
 Keywords: ai,openai,cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: argparse
+Requires-Dist: pyperclip
 
 # Chai - AI in your CLI.
 
 ## Introduction
 
 Chai is a command-line interface (CLI) tool designed to simplify your experience with bash commands. Have you ever found yourself stuck, not knowing the right bash command to use? With Chai, you can simply run `chai [your query in English]`, and it will respond with the appropriate bash command to help you out. 
 
@@ -41,14 +42,22 @@
 
 You can install Chai via pip:
 
 ```
 pip install chai-cli
 ```
 
+### Clipboard
+
+Every output is copied to your clipboard. To ensure that it works, run the following command to install required tools on Linux.
+
+```
+sudo apt-get install xclip xsel wl-clipboard
+```
+
 ## Examples
 
 Here are some examples of queries you can ask Chai:
 
 - "list all files starting with a"
 - "grep emails.txt for yahoo addresses"
 - "list users who are logged in"
```

