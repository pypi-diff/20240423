# Comparing `tmp/dirhash-0.3.0a1.tar.gz` & `tmp/dirhash-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirhash-0.3.0a1.tar", last modified: Tue Apr  9 21:33:24 2024, max compression
+gzip compressed data, was "dirhash-0.4.0.tar", last modified: Tue Apr 23 04:04:22 2024, max compression
```

## Comparing `dirhash-0.3.0a1.tar` & `dirhash-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.483601 dirhash-0.3.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash/
--rw-r--r--   0 runner    (1001) docker     (127)    25634 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/src/dirhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/src/dirhash/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28212 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/tests/test_dirhash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:04:22.926799 dirhash-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 04:04:18.000000 dirhash-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 04:04:18.000000 dirhash-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-23 04:04:22.926799 dirhash-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-23 04:04:18.000000 dirhash-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-23 04:04:18.000000 dirhash-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-23 04:04:22.926799 dirhash-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-23 04:04:18.000000 dirhash-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:04:22.922799 dirhash-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:04:22.926799 dirhash-0.4.0/src/dirhash/
+-rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-04-23 04:04:18.000000 dirhash-0.4.0/src/dirhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 04:04:22.926799 dirhash-0.4.0/src/dirhash/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-23 04:04:18.000000 dirhash-0.4.0/src/dirhash/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:04:22.926799 dirhash-0.4.0/src/dirhash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 04:04:22.000000 dirhash-0.4.0/src/dirhash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:04:22.926799 dirhash-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-23 04:04:18.000000 dirhash-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-23 04:04:18.000000 dirhash-0.4.0/tests/test_dirhash.py
```

### Comparing `dirhash-0.3.0a1/LICENSE` & `dirhash-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a1/PKG-INFO` & `dirhash-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,107 +1,119 @@
 Metadata-Version: 2.1
 Name: dirhash
-Version: 0.3.0a1
+Version: 0.4.0
 Summary: Python module and CLI for hashing of file system directories.
 Home-page: https://github.com/andhus/dirhash-python
 Author: Anders Huss
 Author-email: andhus@kth.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: scantree>=0.0.2
-Requires-Dist: pathspec<0.10.0
+Requires-Dist: scantree
 
 
 [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
 
 # dirhash
+
 A lightweight python module and CLI for computing the hash of any
 directory based on its files' structure and content.
+
 - Supports all hashing algorithms of Python's built-in `hashlib` module.
 - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
 - Multiprocessing for up to [6x speed-up](#performance)
 
 The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
 
 ## Installation
+
 From PyPI:
+
 ```commandline
 pip install dirhash
 ```
+
 Or directly from source:
+
 ```commandline
 git clone git@github.com:andhus/dirhash-python.git
 pip install dirhash/
 ```
 
 ## Usage
+
 Python module:
+
 ```python
 from dirhash import dirhash
 
 dirpath = "path/to/directory"
 dir_md5 = dirhash(dirpath, "md5")
 pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
 no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
 ```
+
 CLI:
+
 ```commandline
 dirhash path/to/directory -a md5
 dirhash path/to/directory -a md5 --match "*.py"
 dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
 ```
 
 ## Why?
+
 If you (or your application) need to verify the integrity of a set of files as well
-as their name and location, you might find this useful. Use-cases range from 
-verification of your image classification dataset (before spending GPU-$$$ on 
+as their name and location, you might find this useful. Use-cases range from
+verification of your image classification dataset (before spending GPU-$$$ on
 training your fancy Deep Learning model) to validation of generated files in
 regression-testing.
 
-There isn't really a standard way of doing this. There are plenty of recipes out 
+There isn't really a standard way of doing this. There are plenty of recipes out
 there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
 and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
-but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
-and documented with a compelling user interface. `dirhash` was created with this as 
+but I couldn't find one that is properly tested (there are some gotcha:s to cover!)
+and documented with a compelling user interface. `dirhash` was created with this as
 the goal.
 
-[checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
+[checksumdir](https://github.com/cakepietoast/checksumdir) is another python
 module/tool with similar intent (that inspired this project) but it lacks much of the
 functionality offered here (most notably including file names/structure in the hash)
 and lacks tests.
 
 ## Performance
+
 The python `hashlib` implementation of common hashing algorithms are highly
-optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
-combines the output. Reasonable measures have been taken to minimize the overhead 
-and for common use-cases, the majority of time is spent reading data from disk 
+optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and
+combines the output. Reasonable measures have been taken to minimize the overhead
+and for common use-cases, the majority of time is spent reading data from disk
 and executing `hashlib` code.
 
 The main effort to boost performance is support for multiprocessing, where the
 reading and hashing is parallelized over individual files.
 
-As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
+As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py)
 with the shell command:
 
-`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
+`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5`
 
-which is the top answer for the SO-question: 
+which is the top answer for the SO-question:
 [Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-Results for two test cases are shown below. Both have 1 GiB of random data: in 
-"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
-"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
+Results for two test cases are shown below. Both have 1 GiB of random data: in
+"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in
+"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories
 in a binary tree of depth 8.
 
-Implementation      | Test Case       | Time (s) | Speed up
-------------------- | --------------- | -------: | -------:
-shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
-`dirhash`           | flat_1k_1MB     | 1.67     | 1.36
-`dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
-shell reference     | nested_32k_32kB | 6.82     | -> 1.0
-`dirhash`           | nested_32k_32kB | 3.43     | 2.00
-`dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
+| Implementation       | Test Case       | Time (s) | Speed up |
+| -------------------- | --------------- | -------: | -------: |
+| shell reference      | flat_1k_1MB     |     2.29 |   -> 1.0 |
+| `dirhash`            | flat_1k_1MB     |     1.67 |     1.36 |
+| `dirhash`(8 workers) | flat_1k_1MB     |     0.48 | **4.73** |
+| shell reference      | nested_32k_32kB |     6.82 |   -> 1.0 |
+| `dirhash`            | nested_32k_32kB |     3.43 |     2.00 |
+| `dirhash`(8 workers) | nested_32k_32kB |     1.14 | **6.00** |
 
 The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
 
 ## Documentation
+
 Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

### Comparing `dirhash-0.3.0a1/README.md` & `dirhash-0.4.0/src/dirhash.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,93 +1,119 @@
+Metadata-Version: 2.1
+Name: dirhash
+Version: 0.4.0
+Summary: Python module and CLI for hashing of file system directories.
+Home-page: https://github.com/andhus/dirhash-python
+Author: Anders Huss
+Author-email: andhus@kth.se
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scantree
+
+
 [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
 
 # dirhash
+
 A lightweight python module and CLI for computing the hash of any
 directory based on its files' structure and content.
+
 - Supports all hashing algorithms of Python's built-in `hashlib` module.
 - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
 - Multiprocessing for up to [6x speed-up](#performance)
 
 The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
 
 ## Installation
+
 From PyPI:
+
 ```commandline
 pip install dirhash
 ```
+
 Or directly from source:
+
 ```commandline
 git clone git@github.com:andhus/dirhash-python.git
 pip install dirhash/
 ```
 
 ## Usage
+
 Python module:
+
 ```python
 from dirhash import dirhash
 
 dirpath = "path/to/directory"
 dir_md5 = dirhash(dirpath, "md5")
 pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
 no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
 ```
+
 CLI:
+
 ```commandline
 dirhash path/to/directory -a md5
 dirhash path/to/directory -a md5 --match "*.py"
 dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
 ```
 
 ## Why?
+
 If you (or your application) need to verify the integrity of a set of files as well
-as their name and location, you might find this useful. Use-cases range from 
-verification of your image classification dataset (before spending GPU-$$$ on 
+as their name and location, you might find this useful. Use-cases range from
+verification of your image classification dataset (before spending GPU-$$$ on
 training your fancy Deep Learning model) to validation of generated files in
 regression-testing.
 
-There isn't really a standard way of doing this. There are plenty of recipes out 
+There isn't really a standard way of doing this. There are plenty of recipes out
 there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
 and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
-but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
-and documented with a compelling user interface. `dirhash` was created with this as 
+but I couldn't find one that is properly tested (there are some gotcha:s to cover!)
+and documented with a compelling user interface. `dirhash` was created with this as
 the goal.
 
-[checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
+[checksumdir](https://github.com/cakepietoast/checksumdir) is another python
 module/tool with similar intent (that inspired this project) but it lacks much of the
 functionality offered here (most notably including file names/structure in the hash)
 and lacks tests.
 
 ## Performance
+
 The python `hashlib` implementation of common hashing algorithms are highly
-optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
-combines the output. Reasonable measures have been taken to minimize the overhead 
-and for common use-cases, the majority of time is spent reading data from disk 
+optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and
+combines the output. Reasonable measures have been taken to minimize the overhead
+and for common use-cases, the majority of time is spent reading data from disk
 and executing `hashlib` code.
 
 The main effort to boost performance is support for multiprocessing, where the
 reading and hashing is parallelized over individual files.
 
-As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
+As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py)
 with the shell command:
 
-`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
+`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5`
 
-which is the top answer for the SO-question: 
+which is the top answer for the SO-question:
 [Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-Results for two test cases are shown below. Both have 1 GiB of random data: in 
-"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
-"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
+Results for two test cases are shown below. Both have 1 GiB of random data: in
+"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in
+"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories
 in a binary tree of depth 8.
 
-Implementation      | Test Case       | Time (s) | Speed up
-------------------- | --------------- | -------: | -------:
-shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
-`dirhash`           | flat_1k_1MB     | 1.67     | 1.36
-`dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
-shell reference     | nested_32k_32kB | 6.82     | -> 1.0
-`dirhash`           | nested_32k_32kB | 3.43     | 2.00
-`dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
+| Implementation       | Test Case       | Time (s) | Speed up |
+| -------------------- | --------------- | -------: | -------: |
+| shell reference      | flat_1k_1MB     |     2.29 |   -> 1.0 |
+| `dirhash`            | flat_1k_1MB     |     1.67 |     1.36 |
+| `dirhash`(8 workers) | flat_1k_1MB     |     0.48 | **4.73** |
+| shell reference      | nested_32k_32kB |     6.82 |   -> 1.0 |
+| `dirhash`            | nested_32k_32kB |     3.43 |     2.00 |
+| `dirhash`(8 workers) | nested_32k_32kB |     1.14 | **6.00** |
 
 The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
 
 ## Documentation
-Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
+
+Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

### Comparing `dirhash-0.3.0a1/setup.py` & `dirhash-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import io
 import os
-from setuptools import setup, find_packages
 
 import versioneer
+from setuptools import find_packages, setup
 
 PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
 
-DESCRIPTION = 'Python module and CLI for hashing of file system directories.'
+DESCRIPTION = "Python module and CLI for hashing of file system directories."
 
 try:
-    with io.open(os.path.join(PROJECT_ROOT, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except IOError:
+    with open(os.path.join(PROJECT_ROOT, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except OSError:
     long_description = DESCRIPTION
 
 setup(
-    name='dirhash',
+    name="dirhash",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/andhus/dirhash-python',
+    url="https://github.com/andhus/dirhash-python",
     author="Anders Huss",
     author_email="andhus@kth.se",
-    license='MIT',
-    install_requires=['scantree>=0.0.2', 'pathspec<0.10.0'],
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
+    license="MIT",
+    install_requires=["scantree"],
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     include_package_data=True,
     entry_points={
-        'console_scripts': ['dirhash=dirhash.cli:main'],
+        "console_scripts": ["dirhash=dirhash.cli:main"],
     },
-    tests_require=['pytest', 'pytest-cov']
+    tests_require=["pre-commit", "pytest", "pytest-cov"],
 )
```

### Comparing `dirhash-0.3.0a1/src/dirhash/__init__.py` & `dirhash-0.4.0/src/dirhash/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 #!/usr/bin/env python
-"""dirhash - a python library (and CLI) for hashing of file system directories.
-"""
-from __future__ import print_function, division
+"""dirhash - a python library (and CLI) for hashing of file system directories."""
 
-import os
 import hashlib
-
+import os
 from functools import partial
 from multiprocessing import Pool
 
-from scantree import (
-    scantree,
-    RecursionFilter,
-    CyclicLinkedDir,
-)
+from scantree import CyclicLinkedDir, RecursionFilter, scantree
 
 from . import _version
-__version__ = _version.get_versions()['version']
+
+__version__ = _version.get_versions()["version"]
 
 __all__ = [
-    '__version__',
-    'algorithms_guaranteed',
-    'algorithms_available',
-    'dirhash',
-    'dirhash_impl',
-    'included_paths',
-    'Filter',
-    'get_match_patterns',
-    'Protocol'
+    "__version__",
+    "algorithms_guaranteed",
+    "algorithms_available",
+    "dirhash",
+    "dirhash_impl",
+    "included_paths",
+    "Filter",
+    "get_match_patterns",
+    "Protocol",
 ]
 
 
-algorithms_guaranteed = {'md5', 'sha1', 'sha224', 'sha256', 'sha384', 'sha512'}
+algorithms_guaranteed = {"md5", "sha1", "sha224", "sha256", "sha384", "sha512"}
 algorithms_available = hashlib.algorithms_available
 
 
 def dirhash(
     directory,
     algorithm,
     match=("*",),
     ignore=None,
     linked_dirs=True,
     linked_files=True,
     empty_dirs=False,
-    entry_properties=('name', 'data'),
+    entry_properties=("name", "data"),
     allow_cyclic_links=False,
     chunk_size=2**20,
-    jobs=1
+    jobs=1,
 ):
     """Computes the hash of a directory based on its structure and content.
 
     # Arguments
         directory: Union[str, pathlib.Path] - Path to the directory to hash.
         algorithm: str - The name of the hashing algorithm to use. See
             `dirhash.algorithms_available` for the available options.
@@ -147,37 +141,31 @@
         See https://github.com/andhus/dirhash/README.md for a formal
         description of how the returned hash value is computed.
     """
     filter_ = Filter(
         match_patterns=get_match_patterns(match=match, ignore=ignore),
         linked_dirs=linked_dirs,
         linked_files=linked_files,
-        empty_dirs=empty_dirs
+        empty_dirs=empty_dirs,
     )
     protocol = Protocol(
-        entry_properties=entry_properties,
-        allow_cyclic_links=allow_cyclic_links
+        entry_properties=entry_properties, allow_cyclic_links=allow_cyclic_links
     )
     return dirhash_impl(
         directory=directory,
         algorithm=algorithm,
         filter_=filter_,
         protocol=protocol,
         chunk_size=chunk_size,
-        jobs=jobs
+        jobs=jobs,
     )
 
 
 def dirhash_impl(
-    directory,
-    algorithm,
-    filter_=None,
-    protocol=None,
-    chunk_size=2**20,
-    jobs=1
+    directory, algorithm, filter_=None, protocol=None, chunk_size=2**20, jobs=1
 ):
     """Computes the hash of a directory based on its structure and content.
 
     In contrast to `dirhash.dirhash`, this function accepts custom implementations of
     the `dirhash.Filter` and `dirhash.Protocol` classes.
 
     # Arguments
@@ -211,57 +199,55 @@
             lead to (infinite) recursion and the protocol option `allow_cyclic_links`
             is `False`.
 
     # References
         See https://github.com/andhus/dirhash/README.md for a formal
         description of how the returned hash value is computed.
     """
+
     def get_instance(value, cls_, argname):
         if isinstance(value, cls_):
             return value
         if value is None:
             return cls_()
-        raise TypeError('{} must be an instance of {} or None'.format(argname, cls_))
+        raise TypeError(f"{argname} must be an instance of {cls_} or None")
 
-    filter_ = get_instance(filter_, Filter, 'filter_')
-    protocol = get_instance(protocol, Protocol, 'protocol')
+    filter_ = get_instance(filter_, Filter, "filter_")
+    protocol = get_instance(protocol, Protocol, "protocol")
     hasher_factory = _get_hasher_factory(algorithm)
 
     def dir_apply(dir_node):
         if not filter_.empty_dirs:
-            if dir_node.path.relative == '' and dir_node.empty:
+            if dir_node.path.relative == "" and dir_node.empty:
                 # only check if root node is empty (other empty dirs are filter
                 # before `dir_apply` with `filter_.empty_dirs=False`)
-                raise ValueError('{}: Nothing to hash'.format(directory))
+                raise ValueError(f"{directory}: Nothing to hash")
         descriptor = protocol.get_descriptor(dir_node)
-        _dirhash = hasher_factory(descriptor.encode('utf-8')).hexdigest()
+        _dirhash = hasher_factory(descriptor.encode("utf-8")).hexdigest()
 
         return dir_node.path, _dirhash
 
     if jobs == 1:
         cache = {}
 
         def file_apply(path):
             return path, _get_filehash(
-                path.real,
-                hasher_factory,
-                chunk_size=chunk_size,
-                cache=cache
+                path.real, hasher_factory, chunk_size=chunk_size, cache=cache
             )
 
         _, dirhash_ = scantree(
             directory,
             recursion_filter=filter_,
             file_apply=file_apply,
             dir_apply=dir_apply,
             follow_links=True,
             allow_cyclic_links=protocol.allow_cyclic_links,
             cache_file_apply=False,
             include_empty=filter_.empty_dirs,
-            jobs=1
+            jobs=1,
         )
     else:  # multiprocessing
         real_paths = set()
 
         def extract_real_paths(path):
             real_paths.add(path.real)
             return path
@@ -270,26 +256,24 @@
             directory,
             recursion_filter=filter_,
             file_apply=extract_real_paths,
             follow_links=True,
             allow_cyclic_links=protocol.allow_cyclic_links,
             cache_file_apply=False,
             include_empty=filter_.empty_dirs,
-            jobs=1
+            jobs=1,
         )
         real_paths = list(real_paths)
         # hash files in parallel
         file_hashes = _parmap(
             partial(
-                _get_filehash,
-                hasher_factory=hasher_factory,
-                chunk_size=chunk_size
+                _get_filehash, hasher_factory=hasher_factory, chunk_size=chunk_size
             ),
             real_paths,
-            jobs=jobs
+            jobs=jobs,
         )
         # prepare the mapping with precomputed file hashes
         real_path_to_hash = dict(zip(real_paths, file_hashes))
 
         def file_apply(path):
             return path, real_path_to_hash[path.real]
 
@@ -320,28 +304,28 @@
         List[str] - A sorted list of the paths that would be included when computing
         the hash of the `directory` using `dirhash.dirhash` and the same arguments.
     """
     filter_ = Filter(
         match_patterns=get_match_patterns(match=match, ignore=ignore),
         linked_dirs=linked_dirs,
         linked_files=linked_files,
-        empty_dirs=empty_dirs
+        empty_dirs=empty_dirs,
     )
     protocol = Protocol(allow_cyclic_links=allow_cyclic_links)
 
     leafpaths = scantree(
         directory,
         recursion_filter=filter_,
         follow_links=True,
         allow_cyclic_links=protocol.allow_cyclic_links,
-        include_empty=filter_.empty_dirs
+        include_empty=filter_.empty_dirs,
     ).leafpaths()
 
     return [
-        path.relative if path.is_file() else os.path.join(path.relative, '.')
+        path.relative if path.is_file() else os.path.join(path.relative, ".")
         for path in leafpaths
     ]
 
 
 class Filter(RecursionFilter):
     """Specification of what files and directories to include for the `dirhash`
     computation.
@@ -360,25 +344,20 @@
         linked_files: bool - If `True` (default), include symbolic linked files in
             the hash computation.
         empty_dirs: bool - If `True`, include empty directories when computing the
             hash. A directory is considered empty if it does not contain any files
             that *matches provided matching criteria*. Default `False`, i.e. empty
             directories are ignored (as is done in git version control).
     """
+
     def __init__(
-        self,
-        match_patterns=None,
-        linked_dirs=True,
-        linked_files=True,
-        empty_dirs=False
+        self, match_patterns=None, linked_dirs=True, linked_files=True, empty_dirs=False
     ):
-        super(Filter, self).__init__(
-            linked_dirs=linked_dirs,
-            linked_files=linked_files,
-            match=match_patterns
+        super().__init__(
+            linked_dirs=linked_dirs, linked_files=linked_files, match=match_patterns
         )
         self.empty_dirs = empty_dirs
 
 
 def get_match_patterns(
     match=None,
     ignore=None,
@@ -396,43 +375,43 @@
             *ignore*. Default `None` (no ignore patterns).
         ignore_extensions: Optional[List[str]] -  A list of file extensions to
             ignore. Short for `ignore=['*.<my extension>', ...]` Default `None` (no
             extensions ignored).
         ignore_hidden: bool - If `True` ignore hidden files and directories. Short
             for `ignore=['.*', '.*/']` Default `False`.
     """
-    match = ['*'] if match is None else list(match)
+    match = ["*"] if match is None else list(match)
     ignore = [] if ignore is None else list(ignore)
     ignore_extensions = [] if ignore_extensions is None else list(ignore_extensions)
 
     if ignore_hidden:
-        ignore.extend(['.*', '.*/'])
+        ignore.extend([".*", ".*/"])
 
     for ext in ignore_extensions:
-        if not ext.startswith('.'):
-            ext = '.' + ext
-        ext = '*' + ext
+        if not ext.startswith("."):
+            ext = "." + ext
+        ext = "*" + ext
         ignore.append(ext)
 
-    match_spec = match + ['!' + ign for ign in ignore]
+    match_spec = match + ["!" + ign for ign in ignore]
 
     def deduplicate(items):
-        items_set = set([])
+        items_set = set()
         dd_items = []
         for item in items:
             if item not in items_set:
                 dd_items.append(item)
                 items_set.add(item)
 
         return dd_items
 
     return deduplicate(match_spec)
 
 
-class Protocol(object):
+class Protocol:
     """Specifications of which file and directory properties to consider when
         computing the `dirhash` value.
 
     # Arguments
         entry_properties: Iterable[str] - A combination of the supported properties
             {"name", "data", "is_link"} where at least one of "name" and "data" is
             included. Interpretation:
@@ -459,72 +438,64 @@
                 will be different than without it even if there are no symbolic links
                 in the directory.
         allow_cyclic_links: bool - If `False` (default) a `SymlinkRecursionError` is
             raised on presence of cyclic symbolic links. If set to `True` the the
             dirhash value for directory causing the cyclic link is replaced with the
             hash function hexdigest of the relative path from the link to the target.
     """
-    class EntryProperties(object):
-        NAME = 'name'
-        DATA = 'data'
-        IS_LINK = 'is_link'
+
+    class EntryProperties:
+        NAME = "name"
+        DATA = "data"
+        IS_LINK = "is_link"
         options = {NAME, DATA, IS_LINK}
-        _DIRHASH = 'dirhash'
+        _DIRHASH = "dirhash"
 
-    _entry_property_separator = '\000'
-    _entry_descriptor_separator = '\000\000'
+    _entry_property_separator = "\000"
+    _entry_descriptor_separator = "\000\000"
 
-    def __init__(
-        self,
-        entry_properties=('name', 'data'),
-        allow_cyclic_links=False
-    ):
+    def __init__(self, entry_properties=("name", "data"), allow_cyclic_links=False):
         entry_properties = set(entry_properties)
         if not entry_properties.issubset(self.EntryProperties.options):
             raise ValueError(
-                'entry properties {} not supported'.format(
-                    entry_properties - self.EntryProperties.options)
+                f"entry properties {entry_properties - self.EntryProperties.options} "
+                "not supported"
             )
         if not (
-            self.EntryProperties.NAME in entry_properties or
-            self.EntryProperties.DATA in entry_properties
+            self.EntryProperties.NAME in entry_properties
+            or self.EntryProperties.DATA in entry_properties
         ):
             raise ValueError(
-                'at least one of entry properties `name` and `data` must be used'
+                "at least one of entry properties `name` and `data` must be used"
             )
         self.entry_properties = entry_properties
         self._include_name = self.EntryProperties.NAME in entry_properties
         self._include_data = self.EntryProperties.DATA in entry_properties
         self._include_is_link = self.EntryProperties.IS_LINK in entry_properties
 
         if not isinstance(allow_cyclic_links, bool):
             raise ValueError(
-                'allow_cyclic_link must be a boolean, '
-                'got {}'.format(allow_cyclic_links)
+                f"allow_cyclic_link must be a boolean, got {allow_cyclic_links}"
             )
         self.allow_cyclic_links = allow_cyclic_links
 
     def get_descriptor(self, dir_node):
         if isinstance(dir_node, CyclicLinkedDir):
             return self._get_cyclic_linked_dir_descriptor(dir_node)
 
         entries = dir_node.directories + dir_node.files
         entry_descriptors = [
-            self._get_entry_descriptor(
-                self._get_entry_properties(path, entry_hash)
-            ) for path, entry_hash in entries
+            self._get_entry_descriptor(self._get_entry_properties(path, entry_hash))
+            for path, entry_hash in entries
         ]
         return self._entry_descriptor_separator.join(sorted(entry_descriptors))
 
     @classmethod
     def _get_entry_descriptor(cls, entry_properties):
-        entry_strings = [
-            '{}:{}'.format(name, value)
-            for name, value in entry_properties
-        ]
+        entry_strings = [f"{name}:{value}" for name, value in entry_properties]
         return cls._entry_property_separator.join(sorted(entry_strings))
 
     def _get_entry_properties(self, path, entry_hash):
         properties = []
         if path.is_dir():
             properties.append((self.EntryProperties._DIRHASH, entry_hash))
         elif self._include_data:  # path is file
@@ -539,16 +510,16 @@
 
     def _get_cyclic_linked_dir_descriptor(self, dir_node):
         relpath = dir_node.path.relative
         target_relpath = dir_node.target_path.relative
         path_to_target = os.path.relpath(
             # the extra '.' is needed if link back to root, because
             # an empty path ('') is not supported by os.path.relpath
-            os.path.join('.', target_relpath),
-            os.path.join('.', relpath)
+            os.path.join(".", target_relpath),
+            os.path.join(".", relpath),
         )
         # TODO normalize posix!
         return path_to_target
 
 
 def _get_hasher_factory(algorithm):
     """Returns a "factory" of hasher instances corresponding to the given algorithm
@@ -558,23 +529,22 @@
     if algorithm in algorithms_guaranteed:
         return getattr(hashlib, algorithm)
 
     if algorithm in algorithms_available:
         return partial(hashlib.new, algorithm)
 
     try:  # bypass algorithm if already a hasher factory
-        hasher = algorithm(b'')
-        hasher.update(b'')
+        hasher = algorithm(b"")
+        hasher.update(b"")
         hasher.hexdigest()
         return algorithm
-    except:
+    except:  # noqa: E722
         pass
 
-    raise ValueError(
-        '`algorithm` must be one of: {}`'.format(algorithms_available))
+    raise ValueError(f"`algorithm` must be one of: {algorithms_available}`")
 
 
 def _parmap(func, iterable, jobs=1):
     """Map with multiprocessing.Pool"""
     if jobs == 1:
         return [func(element) for element in iterable]
 
@@ -610,12 +580,12 @@
         filehash = cache.get(filepath, None)
         if filehash is None:
             filehash = _get_filehash(filepath, hasher_factory, chunk_size)
             cache[filepath] = filehash
         return filehash
 
     hasher = hasher_factory()
-    with open(filepath, 'rb') as f:
-        for chunk in iter(lambda: f.read(chunk_size), b''):
+    with open(filepath, "rb") as f:
+        for chunk in iter(lambda: f.read(chunk_size), b""):
             hasher.update(chunk)
 
     return hasher.hexdigest()
```

### Comparing `dirhash-0.3.0a1/src/dirhash/cli.py` & `dirhash-0.4.0/src/dirhash/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,180 +1,181 @@
 #!/usr/bin/env python
-"""Get hash for the content and/or structure of a directory.
-"""
-from __future__ import print_function
+"""Get hash for the content and/or structure of a directory."""
 
-import sys
 import argparse
+import sys
 
 import dirhash
 
 
 def main():
     try:
         kwargs = get_kwargs(sys.argv[1:])
-        if kwargs.pop('list'):
+        if kwargs.pop("list"):
             # kwargs below have no effect when listing
-            for k in ['algorithm', 'chunk_size', 'jobs', 'entry_properties']:
+            for k in ["algorithm", "chunk_size", "jobs", "entry_properties"]:
                 kwargs.pop(k)
             for leafpath in dirhash.included_paths(**kwargs):
                 print(leafpath)
         else:
             print(dirhash.dirhash(**kwargs))
     except Exception as e:  # pragma: no cover (not picked up by coverage)
-        sys.stderr.write('dirhash: {}\n'.format(e))
+        sys.stderr.write(f"dirhash: {e}\n")
         sys.exit(1)
 
 
 def get_kwargs(args):
-    parser = argparse.ArgumentParser(
-        description='Determine the hash for a directory.'
-    )
-    parser.add_argument(
-        '-v', '--version',
-        action='version',
-        version='dirhash {}'.format(dirhash.__version__)
-    )
+    parser = argparse.ArgumentParser(description="Determine the hash for a directory.")
     parser.add_argument(
-        'directory',
-        help='Directory to hash.'
+        "-v",
+        "--version",
+        action="version",
+        version=f"dirhash {dirhash.__version__}",
     )
+    parser.add_argument("directory", help="Directory to hash.")
     parser.add_argument(
-        '-a', '--algorithm',
+        "-a",
+        "--algorithm",
         choices=dirhash.algorithms_available,
-        default='md5',
+        default="md5",
         help=(
-            'Hashing algorithm to use, by default "md5". Always available: {}. '
-            'Additionally available on current platform: {}. Note that the same '
-            'algorithm may appear multiple times in this set under different names '
-            '(thanks to OpenSSL) '
-            '[https://docs.python.org/2/library/hashlib.html]'.format(
-                sorted(dirhash.algorithms_guaranteed),
-                sorted(dirhash.algorithms_available - dirhash.algorithms_guaranteed)
-            )
+            "Hashing algorithm to use, by default 'md5'. "
+            f"Always available: {sorted(dirhash.algorithms_guaranteed)}. "
+            f"Additionally available on current platform: "
+            f"{sorted(dirhash.algorithms_available - dirhash.algorithms_guaranteed)}. "
+            "Note that the same algorithm may appear multiple times in this set "
+            "under different names (thanks to OpenSSL) "
+            "[https://docs.python.org/2/library/hashlib.html]."
         ),
-        metavar=''
+        metavar="",
     )
 
     filter_options = parser.add_argument_group(
-        title='Filtering options',
+        title="Filtering options",
         description=(
-            'Specify what files and directories to include. All files and '
-            'directories (including symbolic links) are included by default. The '
-            '--match/--ignore arguments allows for selection using glob/wildcard '
+            "Specify what files and directories to include. All files and "
+            "directories (including symbolic links) are included by default. The "
+            "--match/--ignore arguments allows for selection using glob/wildcard "
             '(".gitignore style") path matching. Paths relative to the root '
-            '`directory` (i.e. excluding the name of the root directory itself) are '
-            'matched against the provided patterns. For example, to only include '
+            "`directory` (i.e. excluding the name of the root directory itself) are "
+            "matched against the provided patterns. For example, to only include "
             'python source files, use: `dirhash path/to/dir -m "*.py"` or to '
-            'exclude hidden files and directories use: '
+            "exclude hidden files and directories use: "
             '`dirhash path/to.dir -i ".*" ".*/"` which is short for '
             '`dirhash path/to.dir -m "*" "!.*" "!.*/"`. By adding the --list '
-            'argument, all included paths, for the given filtering arguments, are '
-            'returned instead of the hash value. For further details see '
-            'https://github.com/andhus/dirhash/README.md#filtering'
-        )
+            "argument, all included paths, for the given filtering arguments, are "
+            "returned instead of the hash value. For further details see "
+            "https://github.com/andhus/dirhash/README.md#filtering"
+        ),
     )
     filter_options.add_argument(
-        '-m', '--match',
-        nargs='+',
-        default=['*'],
+        "-m",
+        "--match",
+        nargs="+",
+        default=["*"],
         help=(
-            'One or several patterns for paths to include. NOTE: patterns '
+            "One or several patterns for paths to include. NOTE: patterns "
             'with an asterisk must be in quotes ("*") or the asterisk '
-            'preceded by an escape character (`*).'
+            "preceded by an escape character (`*)."
         ),
-        metavar=''
+        metavar="",
     )
     filter_options.add_argument(
-        '-i', '--ignore',
-        nargs='+',
+        "-i",
+        "--ignore",
+        nargs="+",
         default=None,
         help=(
-            'One or several patterns for paths to exclude. NOTE: patterns '
+            "One or several patterns for paths to exclude. NOTE: patterns "
             'with an asterisk must be in quotes ("*") or the asterisk '
-            'preceded by an escape character (`*).'
+            "preceded by an escape character (`*)."
         ),
-        metavar=''
+        metavar="",
     )
     filter_options.add_argument(
-        '--empty-dirs',
-        action='store_true',
+        "--empty-dirs",
+        action="store_true",
         default=False,
-        help='Include empty directories (containing no files that meet the matching '
-             'criteria and no non-empty sub directories).'
+        help="Include empty directories (containing no files that meet the matching "
+        "criteria and no non-empty sub directories).",
     )
     filter_options.add_argument(
-        '--no-linked-dirs',
-        dest='linked_dirs',
-        action='store_false',
-        help='Do not include symbolic links to other directories.'
+        "--no-linked-dirs",
+        dest="linked_dirs",
+        action="store_false",
+        help="Do not include symbolic links to other directories.",
     )
     filter_options.add_argument(
-        '--no-linked-files',
-        dest='linked_files',
-        action='store_false',
-        help='Do not include symbolic links to files.'
+        "--no-linked-files",
+        dest="linked_files",
+        action="store_false",
+        help="Do not include symbolic links to files.",
     )
     parser.set_defaults(linked_dirs=True, linked_files=True)
 
     protocol_options = parser.add_argument_group(
-        title='Protocol options',
+        title="Protocol options",
         description=(
-            'Specify what properties of files and directories to include and '
-            'whether to allow cyclic links. For further details see '
-            'https://github.com/andhus/dirhash/DIRHASH_STANDARD.md#protocol'
-        )
+            "Specify what properties of files and directories to include and "
+            "whether to allow cyclic links. For further details see "
+            "https://github.com/andhus/dirhash/DIRHASH_STANDARD.md#protocol"
+        ),
     )
     protocol_options.add_argument(
-        '-p', '--properties',
-        nargs='+',
-        dest='entry_properties',
-        default=['data', 'name'],
+        "-p",
+        "--properties",
+        nargs="+",
+        dest="entry_properties",
+        default=["data", "name"],
         help=(
-            'List of file/directory properties to include in the hash. Available '
-            'properties are: {} and at least one of name and data must be '
-            'included. Default is [data name] which means that both the name/paths'
-            ' and content (actual data) of files and directories will be included'
-        ).format(list(dirhash.Protocol.EntryProperties.options)),
-        metavar=''
+            "List of file/directory properties to include in the hash. Available "
+            f"properties are: {list(dirhash.Protocol.EntryProperties.options)} and at "
+            "least one of name and data must be included. Default is [data name] which "
+            "means that both the name/paths and content (actual data) of files and "
+            "directories will be included"
+        ),
+        metavar="",
     )
     protocol_options.add_argument(
-        '-c', '--allow-cyclic-links',
+        "-c",
+        "--allow-cyclic-links",
         default=False,
-        action='store_true',
+        action="store_true",
         help=(
-            'Allow presence of cyclic links (by hashing the relative path to the '
-            'target directory).'
-        )
+            "Allow presence of cyclic links (by hashing the relative path to the "
+            "target directory)."
+        ),
     )
 
     implementation_options = parser.add_argument_group(
-        title='Implementation options',
-        description=''
+        title="Implementation options", description=""
     )
     implementation_options.add_argument(
-        '-s', '--chunk-size',
+        "-s",
+        "--chunk-size",
         default=2**20,
         type=int,
-        help='The chunk size (in bytes) for reading of files.'
+        help="The chunk size (in bytes) for reading of files.",
     )
     implementation_options.add_argument(
-        '-j', '--jobs',
+        "-j",
+        "--jobs",
         type=int,
         default=1,  # TODO make default number of cores?
-        help='Number of jobs (parallel processes) to use.'
+        help="Number of jobs (parallel processes) to use.",
     )
 
-    special_options = parser.add_argument_group(title='Special options')
+    special_options = parser.add_argument_group(title="Special options")
     special_options.add_argument(
-        '-l', '--list',
-        action='store_true',
+        "-l",
+        "--list",
+        action="store_true",
         default=False,
-        help='List the file paths that will be taken into account, given the '
-             'provided filtering options.'
+        help="List the file paths that will be taken into account, given the "
+        "provided filtering options.",
     )
 
     return vars(parser.parse_args(args))
 
 
-if __name__ == '__main__':  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `dirhash-0.3.0a1/src/dirhash.egg-info/PKG-INFO` & `dirhash-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,107 +1,106 @@
-Metadata-Version: 2.1
-Name: dirhash
-Version: 0.3.0a1
-Summary: Python module and CLI for hashing of file system directories.
-Home-page: https://github.com/andhus/dirhash-python
-Author: Anders Huss
-Author-email: andhus@kth.se
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scantree>=0.0.2
-Requires-Dist: pathspec<0.10.0
-
-
 [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
 
 # dirhash
+
 A lightweight python module and CLI for computing the hash of any
 directory based on its files' structure and content.
+
 - Supports all hashing algorithms of Python's built-in `hashlib` module.
 - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
 - Multiprocessing for up to [6x speed-up](#performance)
 
 The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
 
 ## Installation
+
 From PyPI:
+
 ```commandline
 pip install dirhash
 ```
+
 Or directly from source:
+
 ```commandline
 git clone git@github.com:andhus/dirhash-python.git
 pip install dirhash/
 ```
 
 ## Usage
+
 Python module:
+
 ```python
 from dirhash import dirhash
 
 dirpath = "path/to/directory"
 dir_md5 = dirhash(dirpath, "md5")
 pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
 no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
 ```
+
 CLI:
+
 ```commandline
 dirhash path/to/directory -a md5
 dirhash path/to/directory -a md5 --match "*.py"
 dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
 ```
 
 ## Why?
+
 If you (or your application) need to verify the integrity of a set of files as well
-as their name and location, you might find this useful. Use-cases range from 
-verification of your image classification dataset (before spending GPU-$$$ on 
+as their name and location, you might find this useful. Use-cases range from
+verification of your image classification dataset (before spending GPU-$$$ on
 training your fancy Deep Learning model) to validation of generated files in
 regression-testing.
 
-There isn't really a standard way of doing this. There are plenty of recipes out 
+There isn't really a standard way of doing this. There are plenty of recipes out
 there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
 and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
-but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
-and documented with a compelling user interface. `dirhash` was created with this as 
+but I couldn't find one that is properly tested (there are some gotcha:s to cover!)
+and documented with a compelling user interface. `dirhash` was created with this as
 the goal.
 
-[checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
+[checksumdir](https://github.com/cakepietoast/checksumdir) is another python
 module/tool with similar intent (that inspired this project) but it lacks much of the
 functionality offered here (most notably including file names/structure in the hash)
 and lacks tests.
 
 ## Performance
+
 The python `hashlib` implementation of common hashing algorithms are highly
-optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
-combines the output. Reasonable measures have been taken to minimize the overhead 
-and for common use-cases, the majority of time is spent reading data from disk 
+optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and
+combines the output. Reasonable measures have been taken to minimize the overhead
+and for common use-cases, the majority of time is spent reading data from disk
 and executing `hashlib` code.
 
 The main effort to boost performance is support for multiprocessing, where the
 reading and hashing is parallelized over individual files.
 
-As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
+As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py)
 with the shell command:
 
-`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
+`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5`
 
-which is the top answer for the SO-question: 
+which is the top answer for the SO-question:
 [Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-Results for two test cases are shown below. Both have 1 GiB of random data: in 
-"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
-"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
+Results for two test cases are shown below. Both have 1 GiB of random data: in
+"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in
+"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories
 in a binary tree of depth 8.
 
-Implementation      | Test Case       | Time (s) | Speed up
-------------------- | --------------- | -------: | -------:
-shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
-`dirhash`           | flat_1k_1MB     | 1.67     | 1.36
-`dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
-shell reference     | nested_32k_32kB | 6.82     | -> 1.0
-`dirhash`           | nested_32k_32kB | 3.43     | 2.00
-`dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
+| Implementation       | Test Case       | Time (s) | Speed up |
+| -------------------- | --------------- | -------: | -------: |
+| shell reference      | flat_1k_1MB     |     2.29 |   -> 1.0 |
+| `dirhash`            | flat_1k_1MB     |     1.67 |     1.36 |
+| `dirhash`(8 workers) | flat_1k_1MB     |     0.48 | **4.73** |
+| shell reference      | nested_32k_32kB |     6.82 |   -> 1.0 |
+| `dirhash`            | nested_32k_32kB |     3.43 |     2.00 |
+| `dirhash`(8 workers) | nested_32k_32kB |     1.14 | **6.00** |
 
 The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
 
 ## Documentation
+
 Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

### Comparing `dirhash-0.3.0a1/tests/test_cli.py` & `dirhash-0.4.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from __future__ import print_function, division
-
 import os
-import sys
 import shlex
 import subprocess
-
-import dirhash
+import sys
 
 import pytest
 
+import dirhash
 
-console_script = os.path.join(
-    os.path.dirname(sys.executable),
-    'dirhash'
-)
+console_script = os.path.join(os.path.dirname(sys.executable), "dirhash")
 
 
 def dirhash_run(argstring, add_env=None):
     assert os.path.isfile(console_script)
     assert os.access(console_script, os.X_OK)
     if add_env:
         env = os.environ.copy()
         env.update(add_env)
     else:
         env = None
     process = subprocess.Popen(
         [console_script] + shlex.split(argstring),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
-        env=env
+        env=env,
     )
     output, error = process.communicate()
 
     # in python3 output and error are `bytes` as opposed to `str` in python2
     if isinstance(output, bytes):
-        output = output.decode('utf-8')
+        output = output.decode("utf-8")
     if isinstance(error, bytes):
-        error = error.decode('utf-8')
+        error = error.decode("utf-8")
 
     return output, error, process.returncode
 
 
 def create_default_tree(tmpdir):
     """
     tmpdir/
@@ -50,224 +44,197 @@
     |__dir/
     |  |__file
     |__empty/
     |__file
     |__file.ext1
     |__file.ext2
     """
-    dotdir = tmpdir.mkdir('.dir')
-    dotdir.join('file').write('file in hidden sub-directory')
-    tmpdir.join(".file").write('hidden file')
-    dir = tmpdir.mkdir('dir')
-    dir.join('file').write('file in sub-directory')
-    tmpdir.mkdir('empty')
-    tmpdir.join("file").write('file')
-    tmpdir.join("file.ext1").write('file with extension .ext1')
-    tmpdir.join("file.ext2").write('file with extension .ext2')
+    dotdir = tmpdir.mkdir(".dir")
+    dotdir.join("file").write("file in hidden sub-directory")
+    tmpdir.join(".file").write("hidden file")
+    dir = tmpdir.mkdir("dir")
+    dir.join("file").write("file in sub-directory")
+    tmpdir.mkdir("empty")
+    tmpdir.join("file").write("file")
+    tmpdir.join("file.ext1").write("file with extension .ext1")
+    tmpdir.join("file.ext2").write("file with extension .ext2")
 
 
-class TestCLI(object):
+class TestCLI:
     @pytest.mark.parametrize(
-        'argstring, non_default_kwargs',
+        "argstring, non_default_kwargs",
         [
-            (
-                '. -a md5',
-                {}
-            ),
-            (
-                '.. -a md5',
-                {'directory': '..'}
-            ),
-            (
-                'target-dir -a md5',
-                {'directory': 'target-dir'}
-            ),
-            (
-                '. -a sha256',
-                {'algorithm': 'sha256'}
-            ),
+            (". -a md5", {}),
+            (".. -a md5", {"directory": ".."}),
+            ("target-dir -a md5", {"directory": "target-dir"}),
+            (". -a sha256", {"algorithm": "sha256"}),
             # Filtering options
-            (
-                '. -a md5 -m "*" "!.*"',
-                {'match': ['*', '!.*']}
-            ),
+            ('. -a md5 -m "*" "!.*"', {"match": ["*", "!.*"]}),
             (
                 '. -a md5 --match "d1/*" "d2/*" --ignore "*.txt"',
-                {'match': ['d1/*', 'd2/*'], 'ignore': ['*.txt']}
-            ),
-            (
-                '. -a md5 --empty-dirs',
-                {'empty_dirs': True}
-            ),
-            (
-                '. -a md5 --no-linked-dirs',
-                {'linked_dirs': False}
-            ),
-            (
-                '. -a md5 --no-linked-files',
-                {'linked_files': False}
+                {"match": ["d1/*", "d2/*"], "ignore": ["*.txt"]},
             ),
+            (". -a md5 --empty-dirs", {"empty_dirs": True}),
+            (". -a md5 --no-linked-dirs", {"linked_dirs": False}),
+            (". -a md5 --no-linked-files", {"linked_files": False}),
             # Protocol options
-            (
-                '. -a md5 --allow-cyclic-links',
-                {'allow_cyclic_links': True}
-
-            ),
-            (
-                '. -a md5 --properties name',
-                {'entry_properties': ['name']}
-
-            ),
-            (
-                '. -a md5 --properties name data',
-                {'entry_properties': ['name', 'data']}
-
-            ),
+            (". -a md5 --allow-cyclic-links", {"allow_cyclic_links": True}),
+            (". -a md5 --properties name", {"entry_properties": ["name"]}),
+            (". -a md5 --properties name data", {"entry_properties": ["name", "data"]}),
             # Implementation
-            (
-                '. -a md5 -j 10',
-                {'jobs': 10}
-            ),
-            (
-                '. -a md5 -s 32000',
-                {'chunk_size': 32000}
-            ),
-        ]
+            (". -a md5 -j 10", {"jobs": 10}),
+            (". -a md5 -s 32000", {"chunk_size": 32000}),
+        ],
     )
     def test_get_kwargs(self, argstring, non_default_kwargs):
         from dirhash.cli import get_kwargs
+
         kwargs_expected = {
-            'list': False,
-            'directory': '.',
-            'algorithm': 'md5',
-            'match': ['*'],
-            'ignore': None,
-            'empty_dirs': False,
-            'linked_dirs': True,
-            'linked_files': True,
-            'entry_properties': ['data', 'name'],
-            'allow_cyclic_links': False,
-            'chunk_size': 2 ** 20,
-            'jobs': 1
+            "list": False,
+            "directory": ".",
+            "algorithm": "md5",
+            "match": ["*"],
+            "ignore": None,
+            "empty_dirs": False,
+            "linked_dirs": True,
+            "linked_files": True,
+            "entry_properties": ["data", "name"],
+            "allow_cyclic_links": False,
+            "chunk_size": 2**20,
+            "jobs": 1,
         }
         kwargs_expected.update(non_default_kwargs)
         kwargs = get_kwargs(shlex.split(argstring))
         assert kwargs == kwargs_expected
 
     @pytest.mark.parametrize(
-        'description, argstrings, output',
+        "description, argstrings, output",
         [
-            ('ARGS WITHOUT EFFECT WHEN LISTING',
-             ['. -l',
-              '. --list',
-              '. -a md5 --list',
-              '. -a sha256 --list',
-              '. --properties name --list',
-              '. --jobs 2 --list',
-              '. --chunk-size 2 --list'],
-             ('.dir/file\n'
-              '.file\n'
-              'dir/file\n'
-              'file\n'
-              'file.ext1\n'
-              'file.ext2\n')),
-            ('IGNORE EXTENSION',
-             ['. -i "*.ext1" --list',
-              '. --ignore "*.ext1" --list',
-              '. -m "*" "!*.ext1" --list',
-              '. --match "*" "!*.ext1" --list'],
-             ('.dir/file\n'
-              '.file\n'
-              'dir/file\n'
-              'file\n'
-              'file.ext2\n')),
-            ('IGNORE MULTIPLE EXTENSIONS',
-             ['. -i "*.ext1" "*.ext2" --list',
-              '. -i "*.ext*" --list'],
-             ('.dir/file\n'
-              '.file\n'
-              'dir/file\n'
-              'file\n')),
-            ('IGNORE HIDDEN',
-             ['. -i ".*" ".*/" --list'],
-             ('dir/file\n'
-              'file\n'
-              'file.ext1\n'
-              'file.ext2\n')),
-            ('INCLUDE EMPTY',
-             ['. --empty-dirs --list'],
-             ('.dir/file\n'
-              '.file\n'
-              'dir/file\n'
-              'empty/.\n'
-              'file\n'
-              'file.ext1\n'
-              'file.ext2\n')),
-        ]
+            (
+                "ARGS WITHOUT EFFECT WHEN LISTING",
+                [
+                    ". -l",
+                    ". --list",
+                    ". -a md5 --list",
+                    ". -a sha256 --list",
+                    ". --properties name --list",
+                    ". --jobs 2 --list",
+                    ". --chunk-size 2 --list",
+                ],
+                (
+                    ".dir/file\n"
+                    ".file\n"
+                    "dir/file\n"
+                    "file\n"
+                    "file.ext1\n"
+                    "file.ext2\n"
+                ),
+            ),
+            (
+                "IGNORE EXTENSION",
+                [
+                    '. -i "*.ext1" --list',
+                    '. --ignore "*.ext1" --list',
+                    '. -m "*" "!*.ext1" --list',
+                    '. --match "*" "!*.ext1" --list',
+                ],
+                (".dir/file\n" ".file\n" "dir/file\n" "file\n" "file.ext2\n"),
+            ),
+            (
+                "IGNORE MULTIPLE EXTENSIONS",
+                ['. -i "*.ext1" "*.ext2" --list', '. -i "*.ext*" --list'],
+                (".dir/file\n" ".file\n" "dir/file\n" "file\n"),
+            ),
+            (
+                "IGNORE HIDDEN",
+                ['. -i ".*" ".*/" --list'],
+                ("dir/file\n" "file\n" "file.ext1\n" "file.ext2\n"),
+            ),
+            (
+                "INCLUDE EMPTY",
+                [". --empty-dirs --list"],
+                (
+                    ".dir/file\n"
+                    ".file\n"
+                    "dir/file\n"
+                    "empty/.\n"
+                    "file\n"
+                    "file.ext1\n"
+                    "file.ext2\n"
+                ),
+            ),
+        ],
     )
     def test_list(self, description, argstrings, output, tmpdir):
         create_default_tree(tmpdir)
         with tmpdir.as_cwd():
             for argstring in argstrings:
                 o, error, returncode = dirhash_run(argstring)
                 assert returncode == 0
-                assert error == ''
+                assert error == ""
                 assert o == output
 
     @pytest.mark.parametrize(
-        'argstring, kwargs, expected_hashes',
+        "argstring, kwargs, expected_hashes",
         [
-            ('. -a md5',
-             {'algorithm': 'md5'},
-             ['594c48dde0776b03eddeeb0232190be7',
-              'd8ab965636d48e407b73b9dbba4cb928',
-              '050e7bc9ffcb09c15186c04e0f8026df']
-             ),
-            ('. -a sha256',
-             {'algorithm': 'sha256'},
-             ['23a04964149889e932ba3348fe22442f4f6a3b3fec616a386a70579ee857ab7b',
-              '7b76bac43e963f9561f37b96b92d7a174094bff230c6efbf1d8bf650e8b40b7a',
-              '7156da2b2e5a2926eb4b72e65f389343cb6aca0578f0aedcd6f7457abd67d8f5']),
-        ]
+            (
+                ". -a md5",
+                {"algorithm": "md5"},
+                [
+                    "594c48dde0776b03eddeeb0232190be7",
+                    "d8ab965636d48e407b73b9dbba4cb928",
+                    "050e7bc9ffcb09c15186c04e0f8026df",
+                ],
+            ),
+            (
+                ". -a sha256",
+                {"algorithm": "sha256"},
+                [
+                    "23a04964149889e932ba3348fe22442f4f6a3b3fec616a386a70579ee857ab7b",
+                    "7b76bac43e963f9561f37b96b92d7a174094bff230c6efbf1d8bf650e8b40b7a",
+                    "7156da2b2e5a2926eb4b72e65f389343cb6aca0578f0aedcd6f7457abd67d8f5",
+                ],
+            ),
+        ],
     )
     def test_hash_result(self, argstring, kwargs, expected_hashes, tmpdir):
         # verify same result from cmdline and library + regression test of actual
         # hashes
         create_default_tree(tmpdir)
         with tmpdir.as_cwd():
             for add_argstring, add_kwargs, expected_hash in zip(
-                ['', ' -p data', ' -p name'],
+                ["", " -p data", " -p name"],
                 [
                     {},
-                    {'entry_properties': ['data']},
-                    {'entry_properties': ['name']},
+                    {"entry_properties": ["data"]},
+                    {"entry_properties": ["name"]},
                 ],
-                expected_hashes
+                expected_hashes,
             ):
                 # run CLI
                 full_argstring = argstring + add_argstring
                 cli_out, error, returncode = dirhash_run(full_argstring)
-                assert error == ''
+                assert error == ""
                 assert returncode == 0
-                assert cli_out[-1] == '\n'
+                assert cli_out[-1] == "\n"
                 cli_hash = cli_out[:-1]
 
                 # run CLI multiproc
-                full_argstring_mp = argstring + add_argstring + ' --jobs 2'
+                full_argstring_mp = argstring + add_argstring + " --jobs 2"
                 cli_out_mp, error_mp, returncode_mp = dirhash_run(full_argstring_mp)
-                assert error_mp == ''
+                assert error_mp == ""
                 assert returncode_mp == 0
-                assert cli_out_mp[-1] == '\n'
+                assert cli_out_mp[-1] == "\n"
                 cli_hash_mp = cli_out_mp[:-1]
 
                 # run lib function
                 full_kwargs = kwargs.copy()
                 full_kwargs.update(add_kwargs)
                 lib_hash = dirhash.dirhash(str(tmpdir), **full_kwargs)
 
                 assert cli_hash == cli_hash_mp == lib_hash == expected_hash
 
     def test_error_bad_argument(self, tmpdir):
         with tmpdir.as_cwd():
-            o, error, returncode = dirhash_run('. --chunk-size not_an_int')
+            o, error, returncode = dirhash_run(". --chunk-size not_an_int")
             assert returncode > 0
-            assert error != ''
+            assert error != ""
```

### Comparing `dirhash-0.3.0a1/tests/test_dirhash.py` & `dirhash-0.4.0/tests/test_dirhash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,166 +1,158 @@
-from __future__ import print_function, division
-
+import hashlib
 import os
 import shutil
-import hashlib
 import tempfile
 from time import sleep, time
 
 import pytest
+from scantree import SymlinkRecursionError
 
 from dirhash import (
+    Filter,
+    Protocol,
     _get_hasher_factory,
-    get_match_patterns,
-    included_paths,
-    dirhash,
+    _parmap,
     algorithms_available,
     algorithms_guaranteed,
-    Protocol,
-    _parmap,
-    Filter,
-    dirhash_impl
+    dirhash,
+    dirhash_impl,
+    get_match_patterns,
+    included_paths,
 )
-from scantree import SymlinkRecursionError
-
 
-class TestGetHasherFactory(object):
 
+class TestGetHasherFactory:
     def test_get_guaranteed(self):
         algorithm_and_hasher_factory = [
-            ('md5', hashlib.md5),
-            ('sha1', hashlib.sha1),
-            ('sha224', hashlib.sha224),
-            ('sha256', hashlib.sha256),
-            ('sha384', hashlib.sha384),
-            ('sha512', hashlib.sha512)
+            ("md5", hashlib.md5),
+            ("sha1", hashlib.sha1),
+            ("sha224", hashlib.sha224),
+            ("sha256", hashlib.sha256),
+            ("sha384", hashlib.sha384),
+            ("sha512", hashlib.sha512),
         ]
         assert algorithms_guaranteed == {a for a, _ in algorithm_and_hasher_factory}
         for algorithm, expected_hasher_factory in algorithm_and_hasher_factory:
             hasher_factory = _get_hasher_factory(algorithm)
             assert hasher_factory == expected_hasher_factory
 
     def test_get_available(self):
         for algorithm in algorithms_available:
             hasher_factory = _get_hasher_factory(algorithm)
             try:
                 hasher = hasher_factory()
             except ValueError as exc:
-                # Some "available" algorithms are not necessarily available (fails for e.g.
-                # 'ripemd160' in github actions for python 3.8). See:
-                # https://stackoverflow.com/questions/72409563/unsupported-hash-type-ripemd160-with-hashlib-in-python  # noqa
+                # Some "available" algorithms are not necessarily available
+                # (fails for e.g. 'ripemd160' in github actions for python 3.8).
+                # See: https://stackoverflow.com/questions/72409563/unsupported-hash-type-ripemd160-with-hashlib-in-python  # noqa: E501
                 print(f"Failed to create hasher for {algorithm}: {exc}")
                 assert exc.args[0] == f"unsupported hash type {algorithm}"
                 hasher = None
-            
+
             if hasher is not None:
-                assert hasattr(hasher, 'update')
-                assert hasattr(hasher, 'hexdigest')
+                assert hasattr(hasher, "update")
+                assert hasattr(hasher, "hexdigest")
 
     def test_not_available(self):
         with pytest.raises(ValueError):
-            _get_hasher_factory('not available')
+            _get_hasher_factory("not available")
 
     def test_bypass_hasher_factory(self):
-
         # test standard hasher
         hasher_factory = _get_hasher_factory(hashlib.sha256)
         assert hasher_factory is hashlib.sha256
 
         # test raise on custom hasher with bad interface
-        class IncompleteMockHasher(object):
-
+        class IncompleteMockHasher:
             def __init__(self, *args, **kwargs):
                 pass
 
             def update(self, *args, **kwargs):
                 pass
 
         with pytest.raises(ValueError):
             _get_hasher_factory(IncompleteMockHasher)
 
         # test custom hasher with ok interface
         class MockHasher(IncompleteMockHasher):
-
             def hexdigest(self):
-                return ''
+                return ""
 
         hasher_factory = _get_hasher_factory(MockHasher)
         assert hasher_factory is MockHasher
 
 
-class TestGetMatchPatterns(object):
-
+class TestGetMatchPatterns:
     def test_default_match_all(self):
         ms = get_match_patterns()
-        assert ms == ['*']
+        assert ms == ["*"]
 
     def test_only_match(self):
-        ms = get_match_patterns(match=['a*', 'b*'])
-        assert ms == ['a*', 'b*']
+        ms = get_match_patterns(match=["a*", "b*"])
+        assert ms == ["a*", "b*"]
 
     def test_only_ignore(self):
-        ms = get_match_patterns(ignore=['a*', 'b*'])
-        assert ms == ['*', '!a*', '!b*']
+        ms = get_match_patterns(ignore=["a*", "b*"])
+        assert ms == ["*", "!a*", "!b*"]
 
     def test_match_and_ignore(self):
-        ms = get_match_patterns(match=['a*'], ignore=['*.ext'])
-        assert ms == ['a*', '!*.ext']
+        ms = get_match_patterns(match=["a*"], ignore=["*.ext"])
+        assert ms == ["a*", "!*.ext"]
 
     def test_ignore_hidden(self):
         ms = get_match_patterns(ignore_hidden=True)
-        assert ms == ['*', '!.*', '!.*/']
+        assert ms == ["*", "!.*", "!.*/"]
 
         # should not duplicate if present in (general) ignore
-        ms = get_match_patterns(ignore=['.*'], ignore_hidden=True)
-        assert ms == ['*', '!.*', '!.*/']
+        ms = get_match_patterns(ignore=[".*"], ignore_hidden=True)
+        assert ms == ["*", "!.*", "!.*/"]
 
-        ms = get_match_patterns(ignore=['.*/'], ignore_hidden=True)
-        assert ms == ['*', '!.*/', '!.*']
+        ms = get_match_patterns(ignore=[".*/"], ignore_hidden=True)
+        assert ms == ["*", "!.*/", "!.*"]
 
-        ms = get_match_patterns(ignore=['.*', '.*/'], ignore_hidden=True)
-        assert ms == ['*', '!.*', '!.*/']
+        ms = get_match_patterns(ignore=[".*", ".*/"], ignore_hidden=True)
+        assert ms == ["*", "!.*", "!.*/"]
 
     def test_ignore_extensions(self):
-        ms = get_match_patterns(ignore_extensions=['.ext'])
-        assert ms == ['*', '!*.ext']
+        ms = get_match_patterns(ignore_extensions=[".ext"])
+        assert ms == ["*", "!*.ext"]
 
         # automatically adds '.'
-        ms = get_match_patterns(ignore_extensions=['ext'])
-        assert ms == ['*', '!*.ext']
+        ms = get_match_patterns(ignore_extensions=["ext"])
+        assert ms == ["*", "!*.ext"]
 
         # mixed also works
-        ms = get_match_patterns(ignore_extensions=['ext1', '.ext2'])
-        assert ms == ['*', '!*.ext1', '!*.ext2']
+        ms = get_match_patterns(ignore_extensions=["ext1", ".ext2"])
+        assert ms == ["*", "!*.ext1", "!*.ext2"]
 
         # should not duplicate if present in (general) ignore
-        ms = get_match_patterns(ignore=['*.ext'], ignore_extensions=['.ext'])
-        assert ms == ['*', '!*.ext']
+        ms = get_match_patterns(ignore=["*.ext"], ignore_extensions=[".ext"])
+        assert ms == ["*", "!*.ext"]
 
-        ms = get_match_patterns(ignore=['*.ext'], ignore_extensions=['ext'])
-        assert ms == ['*', '!*.ext']
+        ms = get_match_patterns(ignore=["*.ext"], ignore_extensions=["ext"])
+        assert ms == ["*", "!*.ext"]
 
 
-class TempDirTest(object):
-
+class TempDirTest:
     def setup_method(self):
         self.dir = tempfile.mkdtemp()
 
     def teardown_method(self):
         if os.path.exists(self.dir):
             shutil.rmtree(self.dir)
 
     def path_to(self, relpath):
         return os.path.join(self.dir, relpath)
 
     def mkdirs(self, dirpath):
         os.makedirs(self.path_to(dirpath))
 
     def mkfile(self, relpath, content=None):
-        with open(self.path_to(relpath), 'w') as f:
+        with open(self.path_to(relpath), "w") as f:
             if content:
                 f.write(content)
 
     def symlink(self, src, dst):
         os.symlink(self.path_to(src), self.path_to(dst))
 
     def remove(self, relpath):
@@ -169,709 +161,670 @@
         os.remove(self.path_to(relpath))
 
 
 class TestGetIncludedPaths(TempDirTest):
     # Integration tests with `pathspec` for basic use cases.
 
     def test_basic(self):
-        self.mkdirs('root/d1/d11')
-        self.mkdirs('root/d2')
+        self.mkdirs("root/d1/d11")
+        self.mkdirs("root/d2")
 
-        self.mkfile('root/f1')
-        self.mkfile('root/d1/f1')
-        self.mkfile('root/d1/d11/f1')
-        self.mkfile('root/d2/f1')
+        self.mkfile("root/f1")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/d11/f1")
+        self.mkfile("root/d2/f1")
 
-        expected_filepaths = ['d1/d11/f1', 'd1/f1', 'd2/f1', 'f1']
-        filepaths = included_paths(self.path_to('root'))
+        expected_filepaths = ["d1/d11/f1", "d1/f1", "d2/f1", "f1"]
+        filepaths = included_paths(self.path_to("root"))
         assert filepaths == expected_filepaths
 
         # end with '/' or not should not matter
-        filepaths = included_paths(self.path_to('root/'))
+        filepaths = included_paths(self.path_to("root/"))
         assert filepaths == expected_filepaths
 
     def test_not_a_directory(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1')
+        self.mkdirs("root")
+        self.mkfile("root/f1")
         # does not exist
         with pytest.raises(ValueError):
-            included_paths(self.path_to('wrong_root'))
+            included_paths(self.path_to("wrong_root"))
         with pytest.raises(ValueError):
-            included_paths(self.path_to('root/f1'))
+            included_paths(self.path_to("root/f1"))
 
     def test_symlinked_file(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1')
-        self.mkfile('linked_file')
-        self.symlink('linked_file', 'root/f2')
+        self.mkdirs("root")
+        self.mkfile("root/f1")
+        self.mkfile("linked_file")
+        self.symlink("linked_file", "root/f2")
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            linked_files=True
-        )
-        assert filepaths == ['f1', 'f2']
+        filepaths = included_paths(self.path_to("root"), linked_files=True)
+        assert filepaths == ["f1", "f2"]
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            linked_files=False
-        )
-        assert filepaths == ['f1']
+        filepaths = included_paths(self.path_to("root"), linked_files=False)
+        assert filepaths == ["f1"]
 
         # default is 'linked_files': True
-        filepaths = included_paths(self.path_to('root'), )
-        assert filepaths == ['f1', 'f2']
+        filepaths = included_paths(
+            self.path_to("root"),
+        )
+        assert filepaths == ["f1", "f2"]
 
     def test_symlinked_dir(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1')
-        self.mkdirs('linked_dir')
-        self.mkfile('linked_dir/f1')
-        self.mkfile('linked_dir/f2')
-        self.symlink('linked_dir', 'root/d1')
+        self.mkdirs("root")
+        self.mkfile("root/f1")
+        self.mkdirs("linked_dir")
+        self.mkfile("linked_dir/f1")
+        self.mkfile("linked_dir/f2")
+        self.symlink("linked_dir", "root/d1")
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            linked_dirs=False
-        )
-        assert filepaths == ['f1']
+        filepaths = included_paths(self.path_to("root"), linked_dirs=False)
+        assert filepaths == ["f1"]
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            linked_dirs=True
-        )
-        assert filepaths == ['d1/f1', 'd1/f2', 'f1']
+        filepaths = included_paths(self.path_to("root"), linked_dirs=True)
+        assert filepaths == ["d1/f1", "d1/f2", "f1"]
 
         # default is 'linked_dirs': True
-        filepaths = included_paths(self.path_to('root'))
-        assert filepaths == ['d1/f1', 'd1/f2', 'f1']
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == ["d1/f1", "d1/f2", "f1"]
 
     def test_cyclic_link(self):
-        self.mkdirs('root/d1')
-        self.symlink('root', 'root/d1/link_back')
+        self.mkdirs("root/d1")
+        self.symlink("root", "root/d1/link_back")
         with pytest.raises(SymlinkRecursionError) as exc_info:
-            included_paths(
-                self.path_to('root'),
-                allow_cyclic_links=False
-            )
-        assert exc_info.value.real_path == os.path.realpath(self.path_to('root'))
-        assert exc_info.value.first_path == self.path_to('root/')
-        assert exc_info.value.second_path == self.path_to('root/d1/link_back')
-        assert str(exc_info.value).startswith('Symlink recursion:')
+            included_paths(self.path_to("root"), allow_cyclic_links=False)
+        assert exc_info.value.real_path == os.path.realpath(self.path_to("root"))
+        assert exc_info.value.first_path == self.path_to("root/")
+        assert exc_info.value.second_path == self.path_to("root/d1/link_back")
+        assert str(exc_info.value).startswith("Symlink recursion:")
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            allow_cyclic_links=True
-        )
-        assert filepaths == ['d1/link_back/.']
+        filepaths = included_paths(self.path_to("root"), allow_cyclic_links=True)
+        assert filepaths == ["d1/link_back/."]
 
         # default is 'allow_cyclic_links': False
         with pytest.raises(SymlinkRecursionError):
-            filepaths = included_paths(self.path_to('root'))
+            filepaths = included_paths(self.path_to("root"))
+
+    def test_ignore_hidden(self):
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
 
-    def test_ignore_hidden_files(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/.d2')
-
-        self.mkfile('root/f1')
-        self.mkfile('root/.f2')
-        self.mkfile('root/d1/f1')
-        self.mkfile('root/d1/.f2')
-        self.mkfile('root/.d2/f1')
+        self.mkfile("root/f1")
+        self.mkfile("root/.f2")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/.f2")
+        self.mkfile("root/.d2/f1")
 
         # no ignore
-        filepaths = included_paths(self.path_to('root'))
-        assert filepaths == ['.d2/f1', '.f2', 'd1/.f2', 'd1/f1', 'f1']
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == [".d2/f1", ".f2", "d1/.f2", "d1/f1", "f1"]
+
+        # with ignore
+        filepaths = included_paths(self.path_to("root"), match=["*", "!.*"])
+        assert filepaths == ["d1/f1", "f1"]
+
+    def test_ignore_hidden_files_only(self):
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
+
+        self.mkfile("root/f1")
+        self.mkfile("root/.f2")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/.f2")
+        self.mkfile("root/.d2/f1")
+
+        # no ignore
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == [".d2/f1", ".f2", "d1/.f2", "d1/f1", "f1"]
 
         # with ignore
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*']
+            self.path_to("root"), match=["**/*", "!**/.*", "**/.*/*", "!**/.*/.*"]
         )
-        assert filepaths == ['.d2/f1', 'd1/f1', 'f1']
+        assert filepaths == [".d2/f1", "d1/f1", "f1"]
+
+    def test_ignore_hidden_explicitly_recursive(self):
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
+
+        self.mkfile("root/f1")
+        self.mkfile("root/.f2")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/.f2")
+        self.mkfile("root/.d2/f1")
+
+        # no ignore
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == [".d2/f1", ".f2", "d1/.f2", "d1/f1", "f1"]
+
+        # with ignore
+        filepaths = included_paths(self.path_to("root"), match=["*", "!**/.*"])
+        assert filepaths == ["d1/f1", "f1"]
 
     def test_exclude_hidden_dirs(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/.d2')
-        self.mkdirs('root/d1/.d1')
-
-        self.mkfile('root/f1')
-        self.mkfile('root/.f2')
-        self.mkfile('root/d1/f1')
-        self.mkfile('root/d1/.f2')
-        self.mkfile('root/.d2/f1')
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
+        self.mkdirs("root/d1/.d1")
+
+        self.mkfile("root/f1")
+        self.mkfile("root/.f2")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/.f2")
+        self.mkfile("root/.d2/f1")
 
         # no ignore
-        filepaths = included_paths(self.path_to('root'), empty_dirs=True)
-        assert filepaths == ['.d2/f1', '.f2', 'd1/.d1/.', 'd1/.f2', 'd1/f1', 'f1']
+        filepaths = included_paths(self.path_to("root"), empty_dirs=True)
+        assert filepaths == [".d2/f1", ".f2", "d1/.d1/.", "d1/.f2", "d1/f1", "f1"]
 
         # with ignore
-        filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*/']
-        )
-        assert filepaths == ['.f2', 'd1/.f2', 'd1/f1', 'f1']
+        filepaths = included_paths(self.path_to("root"), match=["*", "!.*/"])
+        assert filepaths == [".f2", "d1/.f2", "d1/f1", "f1"]
 
     def test_exclude_hidden_dirs_and_files(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/.d2')
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
 
-        self.mkfile('root/f1')
-        self.mkfile('root/.f2')
-        self.mkfile('root/d1/f1')
-        self.mkfile('root/d1/.f2')
-        self.mkfile('root/.d2/f1')
+        self.mkfile("root/f1")
+        self.mkfile("root/.f2")
+        self.mkfile("root/d1/f1")
+        self.mkfile("root/d1/.f2")
+        self.mkfile("root/.d2/f1")
 
         # no ignore
-        filepaths = included_paths(self.path_to('root'))
-        assert filepaths == ['.d2/f1', '.f2', 'd1/.f2', 'd1/f1', 'f1']
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == [".d2/f1", ".f2", "d1/.f2", "d1/f1", "f1"]
 
         # using ignore
-        filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*/', '!.*']
-        )
-        assert filepaths == ['d1/f1', 'f1']
+        filepaths = included_paths(self.path_to("root"), match=["*", "!.*/", "!.*"])
+        assert filepaths == ["d1/f1", "f1"]
 
     def test_exclude_extensions(self):
-        self.mkdirs('root/d1')
+        self.mkdirs("root/d1")
 
-        self.mkfile('root/f')
-        self.mkfile('root/f.txt')
-        self.mkfile('root/f.skip1')
-        self.mkfile('root/fskip1')
-        self.mkfile('root/f.skip2')
-        self.mkfile('root/f.skip1.txt')
-        self.mkfile('root/f.skip1.skip2')
-        self.mkfile('root/f.skip1skip2')
-        self.mkfile('root/d1/f.txt')
-        self.mkfile('root/d1/f.skip1')
+        self.mkfile("root/f")
+        self.mkfile("root/f.txt")
+        self.mkfile("root/f.skip1")
+        self.mkfile("root/fskip1")
+        self.mkfile("root/f.skip2")
+        self.mkfile("root/f.skip1.txt")
+        self.mkfile("root/f.skip1.skip2")
+        self.mkfile("root/f.skip1skip2")
+        self.mkfile("root/d1/f.txt")
+        self.mkfile("root/d1/f.skip1")
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!*.skip1', '!*.skip2']
+            self.path_to("root"), match=["*", "!*.skip1", "!*.skip2"]
         )
         assert filepaths == [
-            'd1/f.txt', 'f', 'f.skip1.txt', 'f.skip1skip2', 'f.txt', 'fskip1']
+            "d1/f.txt",
+            "f",
+            "f.skip1.txt",
+            "f.skip1skip2",
+            "f.txt",
+            "fskip1",
+        ]
 
     def test_empty_dirs_include_vs_exclude(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/d2')
-        self.mkdirs('root/d3/d31')
-        self.mkdirs('root/d4/d41')
+        self.mkdirs("root/d1")
+        self.mkdirs("root/d2")
+        self.mkdirs("root/d3/d31")
+        self.mkdirs("root/d4/d41")
 
-        self.mkfile('root/d1/f')
-        self.mkfile('root/d3/d31/f')
+        self.mkfile("root/d1/f")
+        self.mkfile("root/d3/d31/f")
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            empty_dirs=False
-        )
-        assert filepaths == ['d1/f', 'd3/d31/f']
+        filepaths = included_paths(self.path_to("root"), empty_dirs=False)
+        assert filepaths == ["d1/f", "d3/d31/f"]
 
         # `include_empty=False` is default
-        filepaths = included_paths(self.path_to('root'))
-        assert filepaths == ['d1/f', 'd3/d31/f']
+        filepaths = included_paths(self.path_to("root"))
+        assert filepaths == ["d1/f", "d3/d31/f"]
 
-        filepaths = included_paths(
-            self.path_to('root'),
-            empty_dirs=True
-        )
-        assert filepaths == ['d1/f', 'd2/.', 'd3/d31/f', 'd4/d41/.']
+        filepaths = included_paths(self.path_to("root"), empty_dirs=True)
+        assert filepaths == ["d1/f", "d2/.", "d3/d31/f", "d4/d41/."]
 
     def test_empty_dirs_because_of_filter_include_vs_exclude(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/d2')
+        self.mkdirs("root/d1")
+        self.mkdirs("root/d2")
 
-        self.mkfile('root/d1/f')
-        self.mkfile('root/d2/.f')
+        self.mkfile("root/d1/f")
+        self.mkfile("root/d2/.f")
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*'],
-            empty_dirs=False
+            self.path_to("root"), match=["*", "!.*"], empty_dirs=False
         )
-        assert filepaths == ['d1/f']
+        assert filepaths == ["d1/f"]
 
         # `include_empty=False` is default
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*'],
+            self.path_to("root"),
+            match=["*", "!.*"],
         )
-        assert filepaths == ['d1/f']
+        assert filepaths == ["d1/f"]
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*'],
-            empty_dirs=True
+            self.path_to("root"), match=["*", "!.*"], empty_dirs=True
         )
-        assert filepaths == ['d1/f', 'd2/.']
+        assert filepaths == ["d1/f", "d2/."]
 
     def test_empty_dir_inclusion_not_affected_by_match(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/.d2')
+        self.mkdirs("root/d1")
+        self.mkdirs("root/.d2")
 
         # NOTE that empty dirs are not excluded by match_patterns:
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*'],
-            empty_dirs=True
+            self.path_to("root"), match=["*", "!.*"], empty_dirs=True
         )
-        assert filepaths == ['.d2/.', 'd1/.']
+        assert filepaths == [".d2/.", "d1/."]
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!.*/'],
-            empty_dirs=True
+            self.path_to("root"), match=["*", "!.*/"], empty_dirs=True
         )
-        assert filepaths == ['.d2/.', 'd1/.']
+        assert filepaths == [".d2/.", "d1/."]
 
         filepaths = included_paths(
-            self.path_to('root'),
-            match=['*', '!d1'],
-            empty_dirs=True
+            self.path_to("root"), match=["*", "!d1"], empty_dirs=True
         )
-        assert filepaths == ['.d2/.', 'd1/.']
+        assert filepaths == [".d2/.", "d1/."]
 
 
 def dirhash_mp_comp(*args, **kwargs):
     res = dirhash(*args, **kwargs)
-    res_mp = dirhash(jobs=2, *args, **kwargs)
+    res_mp = dirhash(*args, **{**kwargs, "jobs": 2})
     assert res == res_mp
     return res
 
 
 class TestDirhash(TempDirTest):
-
     def test_guaranteed_algorithms(self):
-        self.mkdirs('root/d1/d11')
-        self.mkdirs('root/d2')
-        self.mkfile('root/f1', 'a')
-        self.mkfile('root/d1/f1', 'b')
-        self.mkfile('root/d1/d11/f1', 'c')
-        self.mkfile('root/d2/f1', 'd')
+        self.mkdirs("root/d1/d11")
+        self.mkdirs("root/d2")
+        self.mkfile("root/f1", "a")
+        self.mkfile("root/d1/f1", "b")
+        self.mkfile("root/d1/d11/f1", "c")
+        self.mkfile("root/d2/f1", "d")
 
         for algorithm, expected_hash in [
-            ('md5', '3c631c7f5771468a2187494f802fad8f'),
-            ('sha1', '992aa2d00d2ed94f0c19eff7f151f5c6a7e0cc41'),
-            ('sha224', '18013e1df933d5781b2eddb94aceeb7ab689643f1df24060fb478999'),
-            ('sha256', 'ef7e95269fbc0e3478ad31fddd1c7d08'
-                       '907d189c61725332e8a2fd14448fe175'),
-            ('sha384', '64ef4360c172bc68250f9326ea231cd1'
-                       '46a7fa1afe9d386cee0cae0e9f1b4ad2'
-                       '1df050d1df436cff792bbe81d6698026'),
-            ('sha512', '7854226eb0278bc136056998890a8399'
-                       'f85ca383f7c54665026358d28b5dc716'
-                       '0ec654d2bcebf5d60974f82ed820600d'
-                       '8e807ea53d57578d076ec1c82f501208')
+            ("md5", "3c631c7f5771468a2187494f802fad8f"),
+            ("sha1", "992aa2d00d2ed94f0c19eff7f151f5c6a7e0cc41"),
+            ("sha224", "18013e1df933d5781b2eddb94aceeb7ab689643f1df24060fb478999"),
+            (
+                "sha256",
+                "ef7e95269fbc0e3478ad31fddd1c7d08" "907d189c61725332e8a2fd14448fe175",
+            ),
+            (
+                "sha384",
+                "64ef4360c172bc68250f9326ea231cd1"
+                "46a7fa1afe9d386cee0cae0e9f1b4ad2"
+                "1df050d1df436cff792bbe81d6698026",
+            ),
+            (
+                "sha512",
+                "7854226eb0278bc136056998890a8399"
+                "f85ca383f7c54665026358d28b5dc716"
+                "0ec654d2bcebf5d60974f82ed820600d"
+                "8e807ea53d57578d076ec1c82f501208",
+            ),
         ]:
-            hash_value = dirhash_mp_comp(self.path_to('root'), algorithm)
+            hash_value = dirhash_mp_comp(self.path_to("root"), algorithm)
             assert hash_value == expected_hash
 
     def test_recursive_descriptor(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/d2')
-        self.mkfile('root/f1', 'a')
-        self.mkfile('root/d1/f12', 'b')
-
-        f1_desc = 'data:a\000name:f1'
-        f12_desc = 'data:b\000name:f12'
-        d1_desc = 'dirhash:{}\000name:d1'.format(f12_desc)
-        d2_desc = 'dirhash:\000name:d2'
-
-        empty_dirs_false_expected = '\000\000'.join([f1_desc, d1_desc])
-        empty_dirs_true_expected = '\000\000'.join([f1_desc, d2_desc, d1_desc])
-
-        empty_dirs_false = dirhash(
-            self.path_to('root'),
-            algorithm=IdentityHasher
-        )
+        self.mkdirs("root/d1")
+        self.mkdirs("root/d2")
+        self.mkfile("root/f1", "a")
+        self.mkfile("root/d1/f12", "b")
+
+        f1_desc = "data:a\000name:f1"
+        f12_desc = "data:b\000name:f12"
+        d1_desc = f"dirhash:{f12_desc}\000name:d1"
+        d2_desc = "dirhash:\000name:d2"
+
+        empty_dirs_false_expected = "\000\000".join([f1_desc, d1_desc])
+        empty_dirs_true_expected = "\000\000".join([f1_desc, d2_desc, d1_desc])
+
+        empty_dirs_false = dirhash(self.path_to("root"), algorithm=IdentityHasher)
         assert empty_dirs_false == empty_dirs_false_expected
 
         empty_dirs_true = dirhash(
-            self.path_to('root'),
-            algorithm=IdentityHasher,
-            empty_dirs=True
+            self.path_to("root"), algorithm=IdentityHasher, empty_dirs=True
         )
         assert empty_dirs_true == empty_dirs_true_expected
 
     def test_symlinked_file(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/f1', 'a')
-        self.mkfile('linked_file', 'b')
-        self.symlink('linked_file', 'root1/f2')
-
-        self.mkdirs('root2')
-        self.mkfile('root2/f1', 'a')
-        self.mkfile('root2/f2', 'b')
+        self.mkdirs("root1")
+        self.mkfile("root1/f1", "a")
+        self.mkfile("linked_file", "b")
+        self.symlink("linked_file", "root1/f2")
+
+        self.mkdirs("root2")
+        self.mkfile("root2/f1", "a")
+        self.mkfile("root2/f2", "b")
 
         root1_linked_files_true = dirhash_mp_comp(
-            self.path_to('root1'), algorithm='md5'
+            self.path_to("root1"), algorithm="md5"
         )
         root1_linked_files_false = dirhash_mp_comp(
-            self.path_to('root1'), algorithm='md5',
-            linked_files=False
+            self.path_to("root1"), algorithm="md5", linked_files=False
         )
 
-        root2 = dirhash_mp_comp(
-            self.path_to('root2'), algorithm='md5'
-        )
+        root2 = dirhash_mp_comp(self.path_to("root2"), algorithm="md5")
 
         assert root1_linked_files_false != root1_linked_files_true
         assert root1_linked_files_true == root2
 
     def test_symlinked_dir(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/f1', 'a')
-        self.mkdirs('linked_dir')
-        self.mkfile('linked_dir/f1', 'b')
-        self.mkfile('linked_dir/f2', 'c')
-        self.symlink('linked_dir', 'root1/d1')
-
-        self.mkdirs('root2')
-        self.mkfile('root2/f1', 'a')
-        self.mkdirs('root2/d1')
-        self.mkfile('root2/d1/f1', 'b')
-        self.mkfile('root2/d1/f2', 'c')
+        self.mkdirs("root1")
+        self.mkfile("root1/f1", "a")
+        self.mkdirs("linked_dir")
+        self.mkfile("linked_dir/f1", "b")
+        self.mkfile("linked_dir/f2", "c")
+        self.symlink("linked_dir", "root1/d1")
+
+        self.mkdirs("root2")
+        self.mkfile("root2/f1", "a")
+        self.mkdirs("root2/d1")
+        self.mkfile("root2/d1/f1", "b")
+        self.mkfile("root2/d1/f2", "c")
 
         root1_linked_dirs_true = dirhash_mp_comp(
-            self.path_to('root1'),
-            algorithm='md5',
-            linked_dirs=True
+            self.path_to("root1"), algorithm="md5", linked_dirs=True
         )
         root1_linked_dirs_false = dirhash_mp_comp(
-            self.path_to('root1'),
-            algorithm='md5',
-            linked_dirs=False
-        )
-        root2 = dirhash_mp_comp(
-            self.path_to('root2'), algorithm='md5'
+            self.path_to("root1"), algorithm="md5", linked_dirs=False
         )
+        root2 = dirhash_mp_comp(self.path_to("root2"), algorithm="md5")
 
         assert root1_linked_dirs_false != root1_linked_dirs_true
         assert root1_linked_dirs_true == root2
 
     def test_cache_used_for_symlinks(self):
-
-        self.mkdirs('root/dir')
-        self.mkfile('root/file', '< one chunk content')
+        self.mkdirs("root/dir")
+        self.mkfile("root/file", "< one chunk content")
         for i in range(10):
-            self.symlink('root/file', 'root/link_{}'.format(i))
+            self.symlink("root/file", f"root/link_{i}")
         for i in range(10):
-            self.symlink('root/file', 'root/dir/link_{}'.format(i))
+            self.symlink("root/file", f"root/dir/link_{i}")
         start = time()
-        dirhash(self.path_to('root'), algorithm=SlowHasher)
+        dirhash(self.path_to("root"), algorithm=SlowHasher)
         end = time()
         elapsed = end - start
         assert elapsed < SlowHasher.wait_time * 2
 
     def test_raise_on_empty_root_without_include_empty(self):
-        self.mkdirs('root')
+        self.mkdirs("root")
         with pytest.raises(ValueError):
-            dirhash_mp_comp(self.path_to('root'), 'sha256')
+            dirhash_mp_comp(self.path_to("root"), "sha256")
 
     def test_empty_root_include_empty(self):
-        self.mkdirs('root')
-        dirhash_ = dirhash_mp_comp(
-            self.path_to('root'),
-            'sha256',
-            empty_dirs=True
-        )
-        expected_dirhash = hashlib.sha256(''.encode('utf-8')).hexdigest()
+        self.mkdirs("root")
+        dirhash_ = dirhash_mp_comp(self.path_to("root"), "sha256", empty_dirs=True)
+        expected_dirhash = hashlib.sha256(b"").hexdigest()
         assert dirhash_ == expected_dirhash
 
     def test_include_empty(self):
-        self.mkdirs('root/d1')
-        self.mkdirs('root/d2')
-        self.mkfile('root/d1/f')
-
-        args = (self.path_to('root'), 'sha256')
-        dirhash_ = dirhash_mp_comp(
-            *args,
-            empty_dirs=False
-        )
-        dirhash_empty = dirhash_mp_comp(
-            *args,
-            empty_dirs=True
-        )
+        self.mkdirs("root/d1")
+        self.mkdirs("root/d2")
+        self.mkfile("root/d1/f")
+
+        args = (self.path_to("root"), "sha256")
+        dirhash_ = dirhash_mp_comp(*args, empty_dirs=False)
+        dirhash_empty = dirhash_mp_comp(*args, empty_dirs=True)
         assert dirhash_ != dirhash_empty
 
     def test_chunksize(self):
-        self.mkdirs('root')
-        self.mkfile('root/numbers.txt', str(range(1000)))
+        self.mkdirs("root")
+        self.mkfile("root/numbers.txt", str(range(1000)))
 
-        hash_value = dirhash_mp_comp(self.path_to('root'), 'sha256')
+        hash_value = dirhash_mp_comp(self.path_to("root"), "sha256")
         for chunk_size in [2**4, 2**8, 2**16]:
-            assert dirhash_mp_comp(
-                self.path_to('root'),
-                'sha256',
-                chunk_size=chunk_size
-            ) == hash_value
+            assert (
+                dirhash_mp_comp(self.path_to("root"), "sha256", chunk_size=chunk_size)
+                == hash_value
+            )
 
     def test_data_only(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/a.txt', 'abc')
-        self.mkfile('root1/b.txt', 'def')
-        self.mkdirs('root2')
-        self.mkfile('root2/a.txt', 'abc')
-        self.mkfile('root2/c.txt', 'def')
+        self.mkdirs("root1")
+        self.mkfile("root1/a.txt", "abc")
+        self.mkfile("root1/b.txt", "def")
+        self.mkdirs("root2")
+        self.mkfile("root2/a.txt", "abc")
+        self.mkfile("root2/c.txt", "def")
 
-        hash1 = dirhash_mp_comp(self.path_to('root1'), 'sha256')
-        hash2 = dirhash_mp_comp(self.path_to('root2'), 'sha256')
+        hash1 = dirhash_mp_comp(self.path_to("root1"), "sha256")
+        hash2 = dirhash_mp_comp(self.path_to("root2"), "sha256")
         assert hash1 != hash2
 
         # with entry hash remains the same as long as order of files is the
         # same
         [dhash1, dhash2] = [
-            dirhash_mp_comp(
-                self.path_to(root),
-                'sha256',
-                entry_properties=['data']
-            ) for root in ['root1', 'root2']
+            dirhash_mp_comp(self.path_to(root), "sha256", entry_properties=["data"])
+            for root in ["root1", "root2"]
         ]
         assert dhash1 == dhash2
 
     def test_name_only(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/a.txt', 'abc')
-        self.mkfile('root1/b.txt', 'def')
-        self.mkdirs('root2')
-        self.mkfile('root2/a.txt', 'abc')
-        self.mkfile('root2/b.txt', '___')
+        self.mkdirs("root1")
+        self.mkfile("root1/a.txt", "abc")
+        self.mkfile("root1/b.txt", "def")
+        self.mkdirs("root2")
+        self.mkfile("root2/a.txt", "abc")
+        self.mkfile("root2/b.txt", "___")
 
-        hash1 = dirhash_mp_comp(self.path_to('root1'), 'sha256')
-        hash2 = dirhash_mp_comp(self.path_to('root2'), 'sha256')
+        hash1 = dirhash_mp_comp(self.path_to("root1"), "sha256")
+        hash2 = dirhash_mp_comp(self.path_to("root2"), "sha256")
         assert hash1 != hash2
 
         [dhash1, dhash2] = [
-            dirhash_mp_comp(
-                self.path_to(root),
-                'sha256',
-                entry_properties=['name']
-            ) for root in ['root1', 'root2']
+            dirhash_mp_comp(self.path_to(root), "sha256", entry_properties=["name"])
+            for root in ["root1", "root2"]
         ]
         assert dhash1 == dhash2
 
     def test_is_link_property(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/a.txt', 'abc')
-        self.mkfile('root1/b.txt', 'def')
-        self.mkdirs('root2')
-        self.mkfile('b_target', 'def')
-        self.mkfile('root2/a.txt', 'abc')
-        self.symlink('b_target', 'root2/b.txt')
+        self.mkdirs("root1")
+        self.mkfile("root1/a.txt", "abc")
+        self.mkfile("root1/b.txt", "def")
+        self.mkdirs("root2")
+        self.mkfile("b_target", "def")
+        self.mkfile("root2/a.txt", "abc")
+        self.symlink("b_target", "root2/b.txt")
 
-        hash1 = dirhash_mp_comp(self.path_to('root1'), 'sha256')
-        hash2 = dirhash_mp_comp(self.path_to('root2'), 'sha256')
+        hash1 = dirhash_mp_comp(self.path_to("root1"), "sha256")
+        hash2 = dirhash_mp_comp(self.path_to("root2"), "sha256")
         assert hash1 == hash2
 
         for entry_properties in [
-            ['name', 'data', 'is_link'],
-            ['name', 'is_link'],
-            ['data', 'is_link'],
+            ["name", "data", "is_link"],
+            ["name", "is_link"],
+            ["data", "is_link"],
         ]:
             [hash1, hash2] = [
                 dirhash_mp_comp(
-                    self.path_to(root),
-                    'sha256',
-                    entry_properties=entry_properties
-                ) for root in ['root1', 'root2']
+                    self.path_to(root), "sha256", entry_properties=entry_properties
+                )
+                for root in ["root1", "root2"]
             ]
             assert hash1 != hash2
 
     def test_raise_on_not_at_least_one_of_name_and_data(self):
-        self.mkdirs('root1')
-        self.mkfile('root1/a.txt', 'abc')
-        dirhash_mp_comp(self.path_to('root1'), 'sha256')  # check ok
+        self.mkdirs("root1")
+        self.mkfile("root1/a.txt", "abc")
+        dirhash_mp_comp(self.path_to("root1"), "sha256")  # check ok
         with pytest.raises(ValueError):
-            dirhash_mp_comp(
-                self.path_to('root1'),
-                'sha256',
-                entry_properties=[]
-            )
+            dirhash_mp_comp(self.path_to("root1"), "sha256", entry_properties=[])
 
         with pytest.raises(ValueError):
             dirhash_mp_comp(
-                self.path_to('root1'),
-                'sha256',
-                entry_properties=['is_link']
+                self.path_to("root1"), "sha256", entry_properties=["is_link"]
             )
 
     def test_multiproc_speedup(self):
-
-        self.mkdirs('root/dir')
+        self.mkdirs("root/dir")
         num_files = 10
         for i in range(num_files):
-            self.mkfile('root/file_{}'.format(i), '< one chunk content')
+            self.mkfile(f"root/file_{i}", "< one chunk content")
 
         expected_min_elapsed_sequential = SlowHasher.wait_time * num_files
 
         start = time()
-        dirhash(self.path_to('root'), algorithm=SlowHasher)
+        dirhash(self.path_to("root"), algorithm=SlowHasher)
         end = time()
         elapsed_sequential = end - start
         assert elapsed_sequential > expected_min_elapsed_sequential
 
         start = time()
-        dirhash(self.path_to('root'), algorithm=SlowHasher, jobs=num_files)
+        dirhash(self.path_to("root"), algorithm=SlowHasher, jobs=num_files)
         end = time()
         elapsed_muliproc = end - start
         assert elapsed_muliproc < 0.9 * expected_min_elapsed_sequential
         # just check "any speedup", the overhead varies (and is high on Travis)
 
     def test_cache_by_real_path_speedup(self, tmpdir):
         num_links = 10
 
         # reference run without links
-        root1 = tmpdir.join('root1')
+        root1 = tmpdir.join("root1")
         root1.ensure(dir=True)
         for i in range(num_links):
-            file_i = root1.join('file_{}'.format(i))
-            file_i.write('< one chunk content', ensure=True)
+            file_i = root1.join(f"file_{i}")
+            file_i.write("< one chunk content", ensure=True)
 
         wait_time = SlowHasher.wait_time
         expected_min_elapsed_no_links = wait_time * num_links
         start = time()
         dirhash(root1, algorithm=SlowHasher)
         end = time()
         elapsed_no_links = end - start
         assert elapsed_no_links > expected_min_elapsed_no_links
         overhead = elapsed_no_links - expected_min_elapsed_no_links
 
         # all links to same file
-        root2 = tmpdir.join('root2')
+        root2 = tmpdir.join("root2")
         root2.ensure(dir=True)
-        target_file = tmpdir.join('target_file')
+        target_file = tmpdir.join("target_file")
         target_file.ensure()
         for i in range(num_links):
-            root2.join('link_{}'.format(i)).mksymlinkto(target_file)
+            root2.join(f"link_{i}").mksymlinkto(target_file)
 
         overhead_margin_factor = 1.5
         expected_max_elapsed_with_links = overhead * overhead_margin_factor + wait_time
         assert expected_max_elapsed_with_links < expected_min_elapsed_no_links
         start = time()
         dirhash(root2, algorithm=SlowHasher)
         end = time()
         elapsed_with_links = end - start
         assert elapsed_with_links < expected_max_elapsed_with_links
 
     def test_cache_together_with_multiprocess_speedup(self, tmpdir):
-        target_file_names = ['target_file_1', 'target_file_2']
+        target_file_names = ["target_file_1", "target_file_2"]
         num_links_per_file = 10
         num_links = num_links_per_file * len(target_file_names)
 
         # reference run without links
-        root1 = tmpdir.join('root1')
+        root1 = tmpdir.join("root1")
         root1.ensure(dir=True)
         for i in range(num_links):
-            file_i = root1.join('file_{}'.format(i))
-            file_i.write('< one chunk content', ensure=True)
+            file_i = root1.join(f"file_{i}")
+            file_i.write("< one chunk content", ensure=True)
 
         jobs = 2
         wait_time = SlowHasher.wait_time
         expected_min_elapsed_no_links = wait_time * num_links / jobs
         start = time()
         dirhash(root1, algorithm=SlowHasher, jobs=jobs)
         end = time()
         elapsed_no_links = end - start
         assert elapsed_no_links > expected_min_elapsed_no_links
         overhead = elapsed_no_links - expected_min_elapsed_no_links
 
-        root2 = tmpdir.join('root2')
+        root2 = tmpdir.join("root2")
         root2.ensure(dir=True)
         for i, target_file_name in enumerate(target_file_names):
             target_file = tmpdir.join(target_file_name)
-            target_file.write('< one chunk content', ensure=True)
+            target_file.write("< one chunk content", ensure=True)
             for j in range(num_links_per_file):
-                root2.join('link_{}_{}'.format(i, j)).mksymlinkto(target_file)
+                root2.join(f"link_{i}_{j}").mksymlinkto(target_file)
 
         overhead_margin_factor = 1.5
-        expected_max_elapsed_with_links = overhead * overhead_margin_factor + wait_time * 2
+        expected_max_elapsed_with_links = (
+            overhead * overhead_margin_factor + wait_time * 2
+        )
         assert expected_max_elapsed_with_links < expected_min_elapsed_no_links
         start = time()
         dirhash(root2, algorithm=SlowHasher, jobs=jobs)
         end = time()
         elapsed_mp_with_links = end - start
         assert elapsed_mp_with_links < expected_max_elapsed_with_links
 
     def test_hash_cyclic_link_to_root(self):
-        self.mkdirs('root/d1')
-        self.symlink('root', 'root/d1/link_back')
-        dirhash(
-            self.path_to('root'),
-            'sha256',
-            allow_cyclic_links=True
-        )
+        self.mkdirs("root/d1")
+        self.symlink("root", "root/d1/link_back")
+        dirhash(self.path_to("root"), "sha256", allow_cyclic_links=True)
 
     def test_hash_cyclic_link(self):
-        self.mkdirs('root/d1/d2')
-        self.symlink('root/d1', 'root/d1/d2/link_back')
-        dirhash(
-            self.path_to('root'),
-            'sha256',
-            allow_cyclic_links=True
-        )
+        self.mkdirs("root/d1/d2")
+        self.symlink("root/d1", "root/d1/d2/link_back")
+        dirhash(self.path_to("root"), "sha256", allow_cyclic_links=True)
 
     def test_pass_filtering_instance(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1', '')
-        dirhash_impl(self.path_to('root'), 'sha256', filter_=Filter())
+        self.mkdirs("root")
+        self.mkfile("root/f1", "")
+        dirhash_impl(self.path_to("root"), "sha256", filter_=Filter())
 
     def test_pass_protocol_instance(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1', '')
-        dirhash_impl(self.path_to('root'), 'sha256', protocol=Protocol())
+        self.mkdirs("root")
+        self.mkfile("root/f1", "")
+        dirhash_impl(self.path_to("root"), "sha256", protocol=Protocol())
 
     def test_raise_on_wrong_type(self):
-        self.mkdirs('root')
-        self.mkfile('root/f1', '')
+        self.mkdirs("root")
+        self.mkfile("root/f1", "")
         with pytest.raises(TypeError):
-            dirhash_impl(self.path_to('root'), 'sha256', filter_='')
+            dirhash_impl(self.path_to("root"), "sha256", filter_="")
         with pytest.raises(TypeError):
-            dirhash_impl(self.path_to('root'), 'sha256', protocol='')
+            dirhash_impl(self.path_to("root"), "sha256", protocol="")
 
 
-class SlowHasher(object):
+class SlowHasher:
     wait_time = 0.25
 
     def __init__(self, *args, **kwargs):
         pass
 
     def update(self, data):
-        if data != b'':
+        if data != b"":
             sleep(self.wait_time)
 
     def hexdigest(self):
-        return ''
+        return ""
 
 
-class IdentityHasher(object):
-
-    def __init__(self, initial_data=b''):
-        self.datas = [initial_data.decode('utf-8')]
+class IdentityHasher:
+    def __init__(self, initial_data=b""):
+        self.datas = [initial_data.decode("utf-8")]
 
     def update(self, data):
-        self.datas.append(data.decode('utf-8'))
+        self.datas.append(data.decode("utf-8"))
 
     def hexdigest(self):
-        return ''.join(self.datas)
-
+        return "".join(self.datas)
 
-class TestProtocol(object):
 
+class TestProtocol:
     def test_raise_for_invalid_entry_properties(self):
         with pytest.raises(ValueError):
-            Protocol(entry_properties=['not-valid'])
+            Protocol(entry_properties=["not-valid"])
 
     def test_raise_for_invalid_allow_cyclic_links(self):
         with pytest.raises(ValueError):
-            Protocol(allow_cyclic_links='not-valid')
+            Protocol(allow_cyclic_links="not-valid")
 
 
 def mock_func(x):
     return x * 2
 
 
-@pytest.mark.parametrize('jobs', [1, 2, 4])
+@pytest.mark.parametrize("jobs", [1, 2, 4])
 def test_parmap(jobs):
     inputs = [1, 2, 3, 4]
     assert _parmap(mock_func, inputs, jobs=jobs) == [2, 4, 6, 8]
```

