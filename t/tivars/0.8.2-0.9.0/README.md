# Comparing `tmp/tivars-0.8.2.tar.gz` & `tmp/tivars-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tivars-0.8.2.tar", last modified: Sun Oct 29 18:36:38 2023, max compression
+gzip compressed data, was "tivars-0.9.0.tar", last modified: Mon Apr 22 20:06:03 2024, max compression
```

## Comparing `tivars-0.8.2.tar` & `tivars-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.387322 tivars-0.8.2/
--rw-rw-rw-   0        0        0     1093 2023-06-29 00:12:18.000000 tivars-0.8.2/LICENSE
--rw-rw-rw-   0        0        0     9131 2023-10-29 18:36:38.386324 tivars-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     7314 2023-10-29 18:36:01.000000 tivars-0.8.2/README.md
--rw-rw-rw-   0        0        0     1945 2023-10-29 18:36:01.000000 tivars-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-29 18:36:38.387322 tivars-0.8.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.355131 tivars-0.8.2/tivars/
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.363134 tivars-0.8.2/tivars/PIL/
--rw-rw-rw-   0        0        0      509 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/PIL/TI8caPlugin.py
--rw-rw-rw-   0        0        0      529 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/PIL/TI8ciPlugin.py
--rw-rw-rw-   0        0        0      558 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/PIL/TI8xiPlugin.py
--rw-rw-rw-   0        0        0      183 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/PIL/__init__.py
--rw-rw-rw-   0        0        0     3010 2023-10-29 18:36:24.000000 tivars-0.8.2/tivars/PIL/common.py
--rw-rw-rw-   0        0        0      288 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/__init__.py
--rw-rw-rw-   0        0        0    16846 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/data.py
--rw-rw-rw-   0        0        0     4070 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/flags.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.365386 tivars-0.8.2/tivars/models/
--rw-rw-rw-   0        0        0      553 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/models/__init__.py
--rw-rw-rw-   0        0        0     6710 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/models/model.py
--rw-rw-rw-   0        0        0      535 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/models/versions.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.366391 tivars-0.8.2/tivars/tokenizer/
--rw-rw-rw-   0        0        0     2415 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/tokenizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.367390 tivars-0.8.2/tivars/tokenizer/tokens/
--rw-rw-rw-   0        0        0    89045 2023-08-09 23:11:50.000000 tivars-0.8.2/tivars/tokenizer/tokens/73.xml
--rw-rw-rw-   0        0        0   242780 2023-09-13 16:35:44.000000 tivars-0.8.2/tivars/tokenizer/tokens/8X.xml
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.371249 tivars-0.8.2/tivars/tokenizer/tokens/scripts/
--rw-rw-rw-   0        0        0      187 2023-08-22 23:33:46.000000 tivars-0.8.2/tivars/tokenizer/tokens/scripts/__init__.py
--rw-rw-rw-   0        0        0    10400 2023-09-13 16:35:44.000000 tivars-0.8.2/tivars/tokenizer/tokens/scripts/parse.py
--rw-rw-rw-   0        0        0     2370 2023-09-13 16:35:44.000000 tivars-0.8.2/tivars/tokenizer/tokens/scripts/trie.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.382066 tivars-0.8.2/tivars/types/
--rw-rw-rw-   0        0        0     1472 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/__init__.py
--rw-rw-rw-   0        0        0      972 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/appvar.py
--rw-rw-rw-   0        0        0    11959 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/complex.py
--rw-rw-rw-   0        0        0    45249 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/gdb.py
--rw-rw-rw-   0        0        0     5140 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/group.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.385323 tivars-0.8.2/tivars/types/json/
--rw-rw-rw-   0        0        0     2442 2023-06-13 01:24:56.000000 tivars-0.8.2/tivars/types/json/func.default.json
--rw-rw-rw-   0        0        0     2903 2023-06-13 01:24:56.000000 tivars-0.8.2/tivars/types/json/param.default.json
--rw-rw-rw-   0        0        0     1734 2023-06-13 01:24:56.000000 tivars-0.8.2/tivars/types/json/polar.default.json
--rw-rw-rw-   0        0        0     1284 2023-06-13 01:24:56.000000 tivars-0.8.2/tivars/types/json/seq.default.json
--rw-rw-rw-   0        0        0     6362 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/list.py
--rw-rw-rw-   0        0        0     5853 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/matrix.py
--rw-rw-rw-   0        0        0     5019 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/numeric.py
--rw-rw-rw-   0        0        0    11655 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/picture.py
--rw-rw-rw-   0        0        0    18817 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/real.py
--rw-rw-rw-   0        0        0    17341 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/settings.py
--rw-rw-rw-   0        0        0    12642 2023-10-29 05:13:48.000000 tivars-0.8.2/tivars/types/tokenized.py
--rw-rw-rw-   0        0        0    36636 2023-10-29 18:36:01.000000 tivars-0.8.2/tivars/var.py
-drwxrwxrwx   0        0        0        0 2023-10-29 18:36:38.359134 tivars-0.8.2/tivars.egg-info/
--rw-rw-rw-   0        0        0     9131 2023-10-29 18:36:38.000000 tivars-0.8.2/tivars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-10-29 18:36:38.000000 tivars-0.8.2/tivars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-29 18:36:38.000000 tivars-0.8.2/tivars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-10-29 18:36:38.000000 tivars-0.8.2/tivars.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-10-29 18:36:38.000000 tivars-0.8.2/tivars.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.342629 tivars-0.9.0/
+-rw-rw-rw-   0        0        0     1093 2023-12-28 22:35:37.000000 tivars-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0    10710 2024-04-22 20:06:03.342629 tivars-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8893 2024-04-22 20:05:27.000000 tivars-0.9.0/README.md
+-rw-rw-rw-   0        0        0     1897 2024-04-22 20:05:27.000000 tivars-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 20:06:03.342629 tivars-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.320944 tivars-0.9.0/tivars/
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.327261 tivars-0.9.0/tivars/PIL/
+-rw-rw-rw-   0        0        0      509 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8caPlugin.py
+-rw-rw-rw-   0        0        0      529 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8ciPlugin.py
+-rw-rw-rw-   0        0        0      558 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8xiPlugin.py
+-rw-rw-rw-   0        0        0      183 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/__init__.py
+-rw-rw-rw-   0        0        0     3010 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/common.py
+-rw-rw-rw-   0        0        0      309 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/__init__.py
+-rw-rw-rw-   0        0        0    17327 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/data.py
+-rw-rw-rw-   0        0        0     4064 2023-12-31 23:22:16.000000 tivars-0.9.0/tivars/flags.py
+-rw-rw-rw-   0        0        0    25084 2024-04-22 16:40:44.000000 tivars-0.9.0/tivars/flash.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.328287 tivars-0.9.0/tivars/models/
+-rw-rw-rw-   0        0        0      553 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/models/__init__.py
+-rw-rw-rw-   0        0        0     7215 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/models/model.py
+-rw-rw-rw-   0        0        0      523 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/models/versions.py
+-rw-rw-rw-   0        0        0     5136 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/numeric.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.328287 tivars-0.9.0/tivars/tokenizer/
+-rw-rw-rw-   0        0        0     2519 2024-01-03 06:10:34.000000 tivars-0.9.0/tivars/tokenizer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.329662 tivars-0.9.0/tivars/tokens/
+-rw-rw-rw-   0        0        0    89045 2024-01-12 06:13:35.000000 tivars-0.9.0/tivars/tokens/73.xml
+-rw-rw-rw-   0        0        0   243356 2024-01-27 18:37:59.000000 tivars-0.9.0/tivars/tokens/8X.xml
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.332665 tivars-0.9.0/tivars/tokens/scripts/
+-rw-rw-rw-   0        0        0      316 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/__init__.py
+-rw-rw-rw-   0        0        0      677 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/build.py
+-rw-rw-rw-   0        0        0     6516 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/formats.py
+-rw-rw-rw-   0        0        0    10440 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/parse.py
+-rw-rw-rw-   0        0        0     7135 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/tokenide.py
+-rw-rw-rw-   0        0        0     2370 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/trie.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.339090 tivars-0.9.0/tivars/types/
+-rw-rw-rw-   0        0        0     1664 2023-12-31 23:01:25.000000 tivars-0.9.0/tivars/types/__init__.py
+-rw-rw-rw-   0        0        0      977 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/appvar.py
+-rw-rw-rw-   0        0        0    12017 2024-01-13 17:19:27.000000 tivars-0.9.0/tivars/types/complex.py
+-rw-rw-rw-   0        0        0     1780 2024-01-13 17:15:58.000000 tivars-0.9.0/tivars/types/flash.py
+-rw-rw-rw-   0        0        0    45527 2024-04-22 15:19:59.000000 tivars-0.9.0/tivars/types/gdb.py
+-rw-rw-rw-   0        0        0     5188 2024-02-21 18:17:10.000000 tivars-0.9.0/tivars/types/group.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.341125 tivars-0.9.0/tivars/types/json/
+-rw-rw-rw-   0        0        0     2442 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/func.default.json
+-rw-rw-rw-   0        0        0     2903 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/param.default.json
+-rw-rw-rw-   0        0        0     1734 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/polar.default.json
+-rw-rw-rw-   0        0        0     1284 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/seq.default.json
+-rw-rw-rw-   0        0        0     6347 2023-12-30 22:09:28.000000 tivars-0.9.0/tivars/types/list.py
+-rw-rw-rw-   0        0        0     5857 2023-12-30 22:07:29.000000 tivars-0.9.0/tivars/types/matrix.py
+-rw-rw-rw-   0        0        0    11665 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/picture.py
+-rw-rw-rw-   0        0        0    18833 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/real.py
+-rw-rw-rw-   0        0        0    17351 2023-12-30 04:03:46.000000 tivars-0.9.0/tivars/types/settings.py
+-rw-rw-rw-   0        0        0    13624 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/types/tokenized.py
+-rw-rw-rw-   0        0        0    37711 2024-04-22 20:05:27.000000 tivars-0.9.0/tivars/var.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.341125 tivars-0.9.0/tivars.egg-info/
+-rw-rw-rw-   0        0        0    10710 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/top_level.txt
```

### Comparing `tivars-0.8.2/LICENSE` & `tivars-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/PKG-INFO` & `tivars-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tivars
-Version: 0.8.2
+Version: 0.9.0
 Summary: A library for interacting with TI-(e)z80 (82/83/84 series) calculator files
 License: The MIT License (MIT)
         
         Copyright (c) 2023 kg583
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,107 +35,109 @@
 Provides-Extra: arrays
 Requires-Dist: numpy; extra == "arrays"
 
 # tivars_lib_py
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
-Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting).
+Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.8.2`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
 
 Alternatively, you can clone this repository or [download a release](https://github.com/TI-Toolkit/tivars_lib_py/tags) and extract the `tivars` directory to include it in your next project. Once downloaded, you can also use `pip` to install it locally.
 
 ### As a Submodule
 
-Include this repository in your next project as a submodule using `git submodule` or manually cloning and writing the following in `.gitmodules`:
-
-```
-[submodule "tivars_lib_py"]
-	path = path/to/tivars_lib_py
-	url = https://github.com/TI-Toolkit/tivars_lib_py.git
-```
-
-Then, add the following to any file which imports `tivars`:
+Include this repository in your next project as a submodule using the `git submodule` command. Then, add the following to any file which imports `tivars`:
 
 ```py
 import sys
 
 sys.path.insert(1, 'tivars_lib_py/')
 ```
 
 Check out [this tool](https://github.com/TI-Toolkit/token_translation_extractor) for an example.
 
 ### Unit Testing
 
 You can run the test suite via `__main__.py`, or run individual tests found in `tests/` with `unittest`. Tests for optional package extensions (e.g. PIL) will be skipped if the package cannot be found.
 
-Note that the PyPI distribution does _not_ include the test suite.
+> [!WARNING]
+> The PyPI distribution does _not_ include the test suite.
 
 ## How to Use
 
-### Creating vars
+### Creating objects
+
+### Var basics
 
 Every var file has two parts: a _header_ and a number of _entries_, where an entry contains the data for a single variable. Usually, var files contain just one entry; in these cases, there's not much distinction between a var and an entry for the purposes of messing with its data.
 
+### Entries
+
 To create an empty entry, instantiate its corresponding type from `tivars.types`. You can specify additional parameters as you like:
 
 ```python
 from tivars.models import *
 from tivars.types import *
 
 my_program = TIProgram(name="HELLO")
 ```
 
-If you're not sure of an entry's type, instantiate a base `TIEntry`:
+> [!TIP]
+> If you're not sure of an entry's type, you can instantiate a base `TIEntry`.
 
-```python
-my_entry = TIEntry()
-```
+### Vars and Headers
 
 If you want to create an entire var or just a header, use `TIVar` or `TIHeader` instead:
 
 ```python
 from tivars.var import *
 
 my_var = TIVar()
 my_var_for84pce = TIVar(model=TI_84PCE)
 
 my_header = TIHeader()
 my_header_with_a_cool_comment = TIHeader(comment="Wow! I'm a comment!")
 ```
 
-### Reading and writing
+### Reading files
+
+#### Vars
 
 Vars can be loaded from files or raw bytes:
 
 ```python
 my_var = TIVar.open("HELLO.8xp")
 
-# Note binary mode!
 with open("HELLO.8xp", 'rb') as file:
     my_var.load_var_file(file)
     
     file.seek(0)
     my_var.load_bytes(file.read())
 ```
 
+> [!IMPORTANT]
+> When loading from a file object, make sure the file is opened in binary mode.
+
+#### Entries
+
 Entries can be loaded from files or raw bytes. When loading from a file, you may specify which entry to load if there are multiple:
 
 ```python
-# Raises an error if the var has multiple entries; use load_from_file instead
+# Raises an error if the var has multiple entries
 my_program = TIProgram.open("HELLO.8xp")
 
 with open("HELLO.8xp", 'rb') as file:
     # Offset counts the number of entries to skip; defaults to zero
     my_program.load_from_file(file, offset=1)
     
     file.seek(0)
@@ -149,32 +151,46 @@
 my_program.load_string("Disp \"HELLO WORLD!\"")
 
 my_real = TIReal(1.23)
 my_real.load_float(1.23)
 ```
 
 Base `TIEntry` objects, as well other parent types like `TIGDB`, will be automatically coerced to the correct type:
+
 ```python
 # Coerces to a TIProgram
 my_entry = TIEntry.open("HELLO.8xp")
 ```
 
+> [!TIP]
+> Any entry type can be cast to any other by setting the object's `__class__`.
+
+### Exporting objects
+
+#### Vars
+
 Export a var as bytes or straight to a file:
 
 ```python
 my_var.save("HELLO.8xp")
 
 # Infer the filename and extension
 my_var.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_var.bytes())
 ```
 
+> [!IMPORTANT]
+> `.save()` uses the var's name as the filename, saving to the current working directory.
+
+#### Entries
+
 Entries can be passed an explicit header to attach or model to target when exporting:
+
 ```python
 my_program.save("HELLO.8xp")
 my_program.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_program.export(header=my_header).bytes())
 ```
@@ -183,23 +199,20 @@
 
 ```python
 assert my_program.string() == "Disp \"HELLO WORLD!\""
 
 assert my_real.float() == 1.23
 ```
 
-Data types corresponding to built-in Python types can be obtained from the built-in constructors:
-
-```python
-assert str(my_program) == "Disp \"HELLO WORLD!\""
+> [!TIP]
+> Built-in types can be exported to using the standard constructors, e.g. `str(my_program)`.
 
-assert float(my_real) == 1.23
-```
+### Data Manipulation
 
-### Data Sections
+#### Data sections
 
 Vars are comprised of individual _sections_ which represent different forms of data, split across the header and entries. The var itself also contains the total entry length and checksum sections, but these are read-only to prevent file corruption.
 
 You can read and write to individual sections of an entry or header as their "canonical" type:
 
 ```python
 my_header.comment = "This is my (even cooler) comment!"
@@ -215,19 +228,41 @@
 my_gdb.Xmin = TIReal(0)
 
 assert my_gdb.Xmax == TIReal(10)
 ```
 
 Each section is annotated with the expected type.
 
+> [!TIP]
+> Data sections can accept any subtype of their expected type.
+
+#### Raw containers
+
+All vars store their data sections as raw bytes in the format interpreted by the calculator. Access any data section as a member of the `.raw` attribute to view and edit these bytes directly.
+
+```python
+my_header.raw.comment = "This is my (even rawer) comment!".encode('utf-8')
+my_program.raw.archived = b'\x80'
+
+assert my_program.raw.type_id == b'\x05'
+```
+
+> [!WARNING]
+> Edits to read-only bytes like the checksum are reset whenever any other data in the var is updated.
+
 ### Models
 
 All TI-82/83/84 series calcs are represented as `TIModel` objects stored in `tivars.models`. Each model contains its name, metadata, and features; use `has` on a `TIFeature` to check that a model has a given a feature. Models are also used to determine var file extensions and token sheets.
 
-For these reasons, it is _not_ recommended to instantiate your own models.
+### Flash Files
+
+Flash files such as apps, OSes, and certificates can be loaded using the `TIFlashHeader` base class or its children. A flash file is composed of one to three headers (though usually only one); these are not to be confused with var headers. A flash header does _not_ need to be "packaged" into a larger file format like an entry in a regular var; see `TIFlashHeader.open` and `TIFlashHeader.save`.
+
+> [!TIP]
+> Loading flash files into a `TIEntry` probably won't work very well.
 
 ## Other Functionalities
 
 ### PIL
 
 The `tivars.PIL` package can be used to interface with PIL, the Python Imaging Library. Simply import the package to register codecs for each of the TI image types. You can then open such images directly into a PIL `Image`:
 
@@ -237,18 +272,24 @@
 
 img = Image.open("Pic1.8ci")
 img.show()
 ```
 
 ### Tokenization
 
-Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. Support currently exists for all models in the 82/83/84 series as well as the TI-73; PR's concerning the sheets themselves should be directed upstream to [TI-Toolkit/tokens](https://github.com/TI-Toolkit/tokens).
+Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. These functions utilize the [TI-Toolkit token sheets](https://github.com/TI-Toolkit/tokens), which are kept as a submodule in `tivars.tokens`. Support currently exists for all models in the 82/83/84 series; PR's concerning the sheets themselves should be directed upstream.
+
+> [!IMPORTANT]
+> In contrast to some other tokenizers like SourceCoder, tokenization does _not_ depend on whether the content appears inside a BASIC string literal. Text is always assigned to the _longest_ permissible token.
 
 ## Documentation
 
 Library documentation can be found on [GitHub Pages](https://ti-toolkit.github.io/tivars_lib_py/).
 
 The var file format(s) and data sections can be found in a readable format on the [repository wiki](https://github.com/TI-Toolkit/tivars_lib_py/wiki). Much of the information is copied from the [TI-83 Link Guide](http://merthsoft.com/linkguide/ti83+/vars.html), though has been updated to account for color models.
 
+> [!NOTE]
+> The wiki is still a work-in-progress. Why not [contribute a page](https://github.com/TI-Toolkit/tivars_lib_py/wiki)?
+
 ## Examples
 
 You can find more sample code in `examples` that details common operations on each of the entry types. There are also examples for interfacing with popular external libraries (e.g. NumPy, PIL). Contributions welcome!
```

### Comparing `tivars-0.8.2/README.md` & `tivars-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,106 @@
 # tivars_lib_py
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
-Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting).
+Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.8.2`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
 
 Alternatively, you can clone this repository or [download a release](https://github.com/TI-Toolkit/tivars_lib_py/tags) and extract the `tivars` directory to include it in your next project. Once downloaded, you can also use `pip` to install it locally.
 
 ### As a Submodule
 
-Include this repository in your next project as a submodule using `git submodule` or manually cloning and writing the following in `.gitmodules`:
-
-```
-[submodule "tivars_lib_py"]
-	path = path/to/tivars_lib_py
-	url = https://github.com/TI-Toolkit/tivars_lib_py.git
-```
-
-Then, add the following to any file which imports `tivars`:
+Include this repository in your next project as a submodule using the `git submodule` command. Then, add the following to any file which imports `tivars`:
 
 ```py
 import sys
 
 sys.path.insert(1, 'tivars_lib_py/')
 ```
 
 Check out [this tool](https://github.com/TI-Toolkit/token_translation_extractor) for an example.
 
 ### Unit Testing
 
 You can run the test suite via `__main__.py`, or run individual tests found in `tests/` with `unittest`. Tests for optional package extensions (e.g. PIL) will be skipped if the package cannot be found.
 
-Note that the PyPI distribution does _not_ include the test suite.
+> [!WARNING]
+> The PyPI distribution does _not_ include the test suite.
 
 ## How to Use
 
-### Creating vars
+### Creating objects
+
+### Var basics
 
 Every var file has two parts: a _header_ and a number of _entries_, where an entry contains the data for a single variable. Usually, var files contain just one entry; in these cases, there's not much distinction between a var and an entry for the purposes of messing with its data.
 
+### Entries
+
 To create an empty entry, instantiate its corresponding type from `tivars.types`. You can specify additional parameters as you like:
 
 ```python
 from tivars.models import *
 from tivars.types import *
 
 my_program = TIProgram(name="HELLO")
 ```
 
-If you're not sure of an entry's type, instantiate a base `TIEntry`:
+> [!TIP]
+> If you're not sure of an entry's type, you can instantiate a base `TIEntry`.
 
-```python
-my_entry = TIEntry()
-```
+### Vars and Headers
 
 If you want to create an entire var or just a header, use `TIVar` or `TIHeader` instead:
 
 ```python
 from tivars.var import *
 
 my_var = TIVar()
 my_var_for84pce = TIVar(model=TI_84PCE)
 
 my_header = TIHeader()
 my_header_with_a_cool_comment = TIHeader(comment="Wow! I'm a comment!")
 ```
 
-### Reading and writing
+### Reading files
+
+#### Vars
 
 Vars can be loaded from files or raw bytes:
 
 ```python
 my_var = TIVar.open("HELLO.8xp")
 
-# Note binary mode!
 with open("HELLO.8xp", 'rb') as file:
     my_var.load_var_file(file)
     
     file.seek(0)
     my_var.load_bytes(file.read())
 ```
 
+> [!IMPORTANT]
+> When loading from a file object, make sure the file is opened in binary mode.
+
+#### Entries
+
 Entries can be loaded from files or raw bytes. When loading from a file, you may specify which entry to load if there are multiple:
 
 ```python
-# Raises an error if the var has multiple entries; use load_from_file instead
+# Raises an error if the var has multiple entries
 my_program = TIProgram.open("HELLO.8xp")
 
 with open("HELLO.8xp", 'rb') as file:
     # Offset counts the number of entries to skip; defaults to zero
     my_program.load_from_file(file, offset=1)
     
     file.seek(0)
@@ -112,32 +114,46 @@
 my_program.load_string("Disp \"HELLO WORLD!\"")
 
 my_real = TIReal(1.23)
 my_real.load_float(1.23)
 ```
 
 Base `TIEntry` objects, as well other parent types like `TIGDB`, will be automatically coerced to the correct type:
+
 ```python
 # Coerces to a TIProgram
 my_entry = TIEntry.open("HELLO.8xp")
 ```
 
+> [!TIP]
+> Any entry type can be cast to any other by setting the object's `__class__`.
+
+### Exporting objects
+
+#### Vars
+
 Export a var as bytes or straight to a file:
 
 ```python
 my_var.save("HELLO.8xp")
 
 # Infer the filename and extension
 my_var.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_var.bytes())
 ```
 
+> [!IMPORTANT]
+> `.save()` uses the var's name as the filename, saving to the current working directory.
+
+#### Entries
+
 Entries can be passed an explicit header to attach or model to target when exporting:
+
 ```python
 my_program.save("HELLO.8xp")
 my_program.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_program.export(header=my_header).bytes())
 ```
@@ -146,23 +162,20 @@
 
 ```python
 assert my_program.string() == "Disp \"HELLO WORLD!\""
 
 assert my_real.float() == 1.23
 ```
 
-Data types corresponding to built-in Python types can be obtained from the built-in constructors:
-
-```python
-assert str(my_program) == "Disp \"HELLO WORLD!\""
+> [!TIP]
+> Built-in types can be exported to using the standard constructors, e.g. `str(my_program)`.
 
-assert float(my_real) == 1.23
-```
+### Data Manipulation
 
-### Data Sections
+#### Data sections
 
 Vars are comprised of individual _sections_ which represent different forms of data, split across the header and entries. The var itself also contains the total entry length and checksum sections, but these are read-only to prevent file corruption.
 
 You can read and write to individual sections of an entry or header as their "canonical" type:
 
 ```python
 my_header.comment = "This is my (even cooler) comment!"
@@ -178,19 +191,41 @@
 my_gdb.Xmin = TIReal(0)
 
 assert my_gdb.Xmax == TIReal(10)
 ```
 
 Each section is annotated with the expected type.
 
+> [!TIP]
+> Data sections can accept any subtype of their expected type.
+
+#### Raw containers
+
+All vars store their data sections as raw bytes in the format interpreted by the calculator. Access any data section as a member of the `.raw` attribute to view and edit these bytes directly.
+
+```python
+my_header.raw.comment = "This is my (even rawer) comment!".encode('utf-8')
+my_program.raw.archived = b'\x80'
+
+assert my_program.raw.type_id == b'\x05'
+```
+
+> [!WARNING]
+> Edits to read-only bytes like the checksum are reset whenever any other data in the var is updated.
+
 ### Models
 
 All TI-82/83/84 series calcs are represented as `TIModel` objects stored in `tivars.models`. Each model contains its name, metadata, and features; use `has` on a `TIFeature` to check that a model has a given a feature. Models are also used to determine var file extensions and token sheets.
 
-For these reasons, it is _not_ recommended to instantiate your own models.
+### Flash Files
+
+Flash files such as apps, OSes, and certificates can be loaded using the `TIFlashHeader` base class or its children. A flash file is composed of one to three headers (though usually only one); these are not to be confused with var headers. A flash header does _not_ need to be "packaged" into a larger file format like an entry in a regular var; see `TIFlashHeader.open` and `TIFlashHeader.save`.
+
+> [!TIP]
+> Loading flash files into a `TIEntry` probably won't work very well.
 
 ## Other Functionalities
 
 ### PIL
 
 The `tivars.PIL` package can be used to interface with PIL, the Python Imaging Library. Simply import the package to register codecs for each of the TI image types. You can then open such images directly into a PIL `Image`:
 
@@ -200,18 +235,24 @@
 
 img = Image.open("Pic1.8ci")
 img.show()
 ```
 
 ### Tokenization
 
-Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. Support currently exists for all models in the 82/83/84 series as well as the TI-73; PR's concerning the sheets themselves should be directed upstream to [TI-Toolkit/tokens](https://github.com/TI-Toolkit/tokens).
+Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. These functions utilize the [TI-Toolkit token sheets](https://github.com/TI-Toolkit/tokens), which are kept as a submodule in `tivars.tokens`. Support currently exists for all models in the 82/83/84 series; PR's concerning the sheets themselves should be directed upstream.
+
+> [!IMPORTANT]
+> In contrast to some other tokenizers like SourceCoder, tokenization does _not_ depend on whether the content appears inside a BASIC string literal. Text is always assigned to the _longest_ permissible token.
 
 ## Documentation
 
 Library documentation can be found on [GitHub Pages](https://ti-toolkit.github.io/tivars_lib_py/).
 
 The var file format(s) and data sections can be found in a readable format on the [repository wiki](https://github.com/TI-Toolkit/tivars_lib_py/wiki). Much of the information is copied from the [TI-83 Link Guide](http://merthsoft.com/linkguide/ti83+/vars.html), though has been updated to account for color models.
 
+> [!NOTE]
+> The wiki is still a work-in-progress. Why not [contribute a page](https://github.com/TI-Toolkit/tivars_lib_py/wiki)?
+
 ## Examples
 
 You can find more sample code in `examples` that details common operations on each of the entry types. There are also examples for interfacing with popular external libraries (e.g. NumPy, PIL). Contributions welcome!
```

### Comparing `tivars-0.8.2/pyproject.toml` & `tivars-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.package-data]
 "*" = ["*.default.json", "*.xml"]
 
 
 [project]
 name = "tivars"
-version = "0.8.2"
+version = "0.9.0"
 description = "A library for interacting with TI-(e)z80 (82/83/84 series) calculator files"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 
 [project.urls]
 Repository = "https://github.com/TI-Toolkit/tivars_lib_py"
@@ -44,12 +44,12 @@
 
            "PRIVATE:tivars.data.View.__*__",
            "PUBLIC:tivars.data.View.__init__", "PUBLIC:tivars.data.View.__copy__", "PUBLIC:tivars.data.View.__getitem__",
 
            "PRIVATE:tivars.models.model.*",
            "PUBLIC:tivars.models.model.TIFeature", "PUBLIC:tivars.models.model.TIModel",
 
-           "PRIVATE:tivars.types.numeric.*",
-           "PUBLIC:tivars.types.numeric.BCD", "PUBLIC:tivars.types.numeric.LeftNibbleBCD", "PUBLIC:tivars.types.numeric.RightNibbleBCD",
-           "PUBLIC:tivars.types.numeric.replacer", "PUBLIC:tivars.types.numeric.sign", "PUBLIC:tivars.types.numeric.squash",
-           "PUBLIC:tivars.types.numeric.pi"
+           "PRIVATE:tivars.numeric.*",
+           "PUBLIC:tivars.numeric.BCD", "PUBLIC:tivars.numeric.LeftNibbleBCD", "PUBLIC:tivars.numeric.RightNibbleBCD",
+           "PUBLIC:tivars.numeric.replacer", "PUBLIC:tivars.numeric.sign", "PUBLIC:tivars.numeric.squash",
+           "PUBLIC:tivars.numeric.pi"
 ]
```

### Comparing `tivars-0.8.2/tivars/PIL/TI8ciPlugin.py` & `tivars-0.9.0/tivars/PIL/TI8ciPlugin.py`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/PIL/TI8xiPlugin.py` & `tivars-0.9.0/tivars/PIL/TI8xiPlugin.py`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/PIL/common.py` & `tivars-0.9.0/tivars/PIL/common.py`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/data.py` & `tivars-0.9.0/tivars/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Data interfaces for var objects
 
 This module implements two primary means of data interface:
 
     -   The `Converter` system, which uses the descriptor protocol to treat var data sections as their canonical types.
 
         Each data section of a var, while stored as raw bytes, can be interpreted as some other useful type.
-        Each `Converter` class implements a conversion to such a type, such as ``bytes`` <-> ``str`` using utf-8.
+        Each `Converter` class implements a conversion to such a type, such as ``bytes`` <-> ``str`` using latin-1.
         A data section is declared as either a base `Section` or a `View` into another section and assigned a converter.
         The system allows a user to access data sections as regular variables without cumbersome getters or setters.
 
         See the `Converter` class and its children, and the `Section` and `View` classes for implementation details.
 
     -   The `Loader` system, which implements convenient object initialization using existing mutation methods.
 
@@ -162,15 +162,15 @@
 
     @classmethod
     def set(cls, value: _T, **kwargs) -> bytes:
         """
         Converts ``bool`` -> ``bytes``, where ``b'\\x80'`` is truthy and ``b'\\x00'`` is falsy
 
         :param value: The value to convert
-        :return: ``b'\\x80'`` if ``value` is truthy else ``b'\\x00'``
+        :return: ``b'\\x80'`` if ``value`` is truthy else ``b'\\x00'``
         """
 
         return b'\x80' if value else b'\x00'
 
 
 class Integer(Converter):
     """
@@ -198,47 +198,52 @@
         Converts ``int`` -> ``bytes``
 
         :param value: The value to convert
         :param length: The length of the data section
         :return: The little-endian representation of ``value``
         """
 
-        return int.to_bytes(value, length if length is not None else 2, 'little')
+        length = length if length is not None else 2
+        try:
+            return int.to_bytes(value, length, 'little')
+
+        except OverflowError:
+            raise OverflowError(f"{value} cannot fit in a section of width {length}")
 
 
 class String(Converter):
     """
     Converter for data sections best interpreted as strings
 
-    Strings are encoded in utf-8.
+    Strings are encoded in latin-1.
     """
 
     _T = str
 
     @classmethod
     def get(cls, data: bytes, **kwargs) -> _T:
         """
         Converts ``bytes`` -> ``str``
 
         :param data: The raw bytes to convert
-        :return: The utf-8 decoding of ``data`` with trailing null bytes removed
+        :return: The latin-1 decoding of ``data`` with trailing null bytes removed
         """
 
-        return data.decode('utf8').rstrip('\0')
+        return data.decode('latin-1').rstrip('\0')
 
     @classmethod
     def set(cls, value: _T, **kwargs) -> bytes:
         """
         Converts ``str`` -> ``bytes``
 
         :param value: The value to convert
-        :return: The utf-8 encoding of ``value``
+        :return: The latin-1 encoding of ``value``
         """
 
-        return value.encode('utf8')
+        return value.encode('latin-1')
 
 
 class Bits:
     """
     Sliceable converter to extract and package a slice of bits within a byte
 
     Use like ``Bits[start:end:step]`` to view a slice of a byte.
@@ -291,14 +296,23 @@
                 for index in range(8):
                     if index in indices:
                         data += int(next(bits)) << index
 
                     else:
                         data += current[0] & (1 << index)
 
+                try:
+                    while 1:
+                        if next(bits) == "1":
+                            warn(f"Value {value} has too many bits for this buffer.",
+                                 BytesWarning)
+
+                except StopIteration:
+                    pass
+
                 return bytes([data])
 
         return BitSlice
 
 
 class Section:
     """
```

### Comparing `tivars-0.8.2/tivars/flags.py` & `tivars-0.9.0/tivars/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,43 +24,43 @@
 class Enum(Converter):
     """
     Base class for enum types
 
     This implementation is used over Python's builtin solutions to permit interface with the `Converter` system.
     """
 
-    _T = bytes
+    _T = int
 
     _all = []
 
     @classmethod
     def get(cls, data: bytes, **kwargs) -> _T:
         """
-        Converts ``bytes`` -> ``bytes``, returning the first byte
+        Converts ``bytes`` -> ``int``, returning the first byte
 
         :param data: The raw bytes to convert
         :return: The first byte of ``data``
         """
 
-        return bytes(data[0:1])
+        return data[0]
 
     @classmethod
     def set(cls, value: _T, **kwargs) -> bytes:
         """
-        Converts ``bytes`` -> ``bytes``, enforcing that the input is a recognized enum value
+        Converts ``int`` -> ``bytes``, enforcing that the input is a recognized enum value
 
         :param value: The value to convert
         :return: The byte in ``value``, unchanged
         """
 
         if value not in cls._all:
             warn(f"{value} is not recognized.",
                  BytesWarning)
 
-        return value
+        return bytes([value])
 
     @classmethod
     def get_name(cls, value: _T) -> str:
         """
         Finds the first name in this enum with a given value
 
         :param value: The value to find
```

### Comparing `tivars-0.8.2/tivars/models/__init__.py` & `tivars-0.9.0/tivars/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/models/model.py` & `tivars-0.9.0/tivars/models/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 
 import os
 
 from functools import total_ordering
 
-from ..flags import *
-from ..tokenizer.tokens.scripts import OsVersion, Tokens, TokenTrie
-from ..tokenizer.tokens.scripts.parse import MODEL_ORDER
+from tivars.flags import *
+from tivars.tokens.scripts import OsVersion, Tokens, TokenTrie
+from tivars.tokens.scripts.parse import MODEL_ORDER
 
 
 @total_ordering
 class TIModel:
     """
     Data type for all model constants
 
@@ -31,15 +31,15 @@
     def __init__(self, name: str, features: 'TIFeature', magic: str, product_id: int, lang: str):
         self._name = name
         self._features = TIFeature(features)
         self._magic = magic
         self._product_id = product_id
         self._lang = lang
 
-        with open(os.path.join(os.path.dirname(__file__), "../tokenizer/tokens/8X.xml"), encoding="UTF-8") as file:
+        with open(os.path.join(os.path.dirname(__file__), "../tokens/8X.xml"), encoding="UTF-8") as file:
             self._tokens = Tokens.from_xml_string(file.read(), self.OS("latest"))
 
         self._trie = {}
         for lang in self._tokens.langs:
             self._trie[lang] = TokenTrie.from_tokens(self._tokens, lang)
 
         self._trie[None] = self._trie["en"]
@@ -145,30 +145,61 @@
 
 class TIFeature(Flags):
     """
     Flags representing all calculator features
     """
 
     Complex = {0: 1}
+    """
+    Whether the model supports complex numbers
+    """
+
     Flash = {1: 1}
+    """
+    Whether the model has a flash chip
+    """
+
     Apps = {2: 1}
+    """
+    Whether the model supports apps
+    """
+
     Clock = {3: 1}
+    """
+    Whether the model has a real-time clock
+    """
+
     Color = {4: 1}
-    ez80 = {5: 1}
+    """
+    Whether the model has a color display
+    """
+
+    eZ80 = {5: 1}
+    """
+    Whether the model has an eZ80 chip
+    """
+
     ExactMath = {6: 1}
+    """
+    Whether the model supports exact math for fractions and radicals
+    """
+
     Python = {7: 1}
+    """
+    Whether the model supports Python
+    """
 
 
 features82 = {}
 features83 = features82 | TIFeature.Complex
 features82a = features83 | TIFeature.Flash
 features83p = features82a | TIFeature.Apps
 features84p = features83p | TIFeature.Clock
 features84pcse = features84p | TIFeature.Color
-features84pce = features84pcse | TIFeature.ez80
+features84pce = features84pcse | TIFeature.eZ80
 features83pce = features84pce | TIFeature.ExactMath
 features83pceep = features83pce | TIFeature.Python
 features84pcepy = features84pce | TIFeature.Python
 features82aep = features83pceep | {2: 0}
 
 it = iter(MODEL_ORDER)
 next(it)
```

### Comparing `tivars-0.8.2/tivars/models/versions.py` & `tivars-0.9.0/tivars/models/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 OS version definitions
 """
 
 
-import tivars.tokenizer.tokens.scripts.parse as parse
-
+import tivars.tokens.scripts.parse as parse
 from .model import *
 
 
 class OsVersions(parse.OsVersions):
     """
     Namespace containing useful OS versions
```

### Comparing `tivars-0.8.2/tivars/tokenizer/__init__.py` & `tivars-0.9.0/tivars/tokenizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
-Tokenization utilities derived from the token sheets
+Tokenization utilities derived from the token sheets (see tokens directory)
 """
 
 
-from typing import ByteString
-
 from tivars.data import String
-from ..models import *
-from .tokens.scripts import *
+from tivars.models import *
+from tivars.tokens.scripts import *
 
 
-def decode(bytestream: ByteString, *,
+def decode(bytestream: bytes, *,
            tokens: Tokens = None, lang: str = "en",
            mode: str = "display") -> tuple[str | bytes, OsVersion]:
     tokens = tokens or TI_84PCE.tokens
 
     out = []
     since = OsVersions.INITIAL
 
@@ -33,14 +31,17 @@
             elif len(curr_bytes) >= 2:
                 if not any(key.startswith(curr_bytes[:1]) for key in tokens.bytes):
                     raise ValueError(f"unrecognized byte '0x{curr_bytes[0]:x}' at position {index}")
 
                 else:
                     raise ValueError(f"unrecognized bytes '0x{curr_bytes[0]:x}{curr_bytes[1]:x}' at position {index}")
 
+        elif any(curr_bytes):
+            raise ValueError(f"unexpected null byte at position {index}")
+
         index += 1
 
     return b''.join(out) if mode == "ti_ascii" else "".join(out), since
 
 
 def encode(string: str, trie: TokenTrie) -> tuple[bytes, OsVersion]:
     data = b''
```

### Comparing `tivars-0.8.2/tivars/tokenizer/tokens/73.xml` & `tivars-0.9.0/tivars/tokens/73.xml`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/tokenizer/tokens/8X.xml` & `tivars-0.9.0/tivars/tokens/8X.xml`

 * *Files 0% similar despite different names*

#### Comparing `tivars-0.8.2/tivars/tokenizer/tokens/8X.xml` & `tivars-0.9.0/tivars/tokens/8X.xml`

```diff
@@ -6786,16 +6786,15 @@
       <version>
         <since>
           <model>TI-83+</model>
           <os-version>1.03</os-version>
         </since>
         <lang code="en" ti-ascii="B7">
           <display>`</display>
-          <accessible>`</accessible>
-          <variant>|`</variant>
+          <accessible>|`</accessible>
           <variant>^^`</variant>
         </lang>
       </version>
     </token>
     <token value="$9C">
       <version>
         <since>
@@ -7826,17 +7825,16 @@
     <token value="$F5">
       <version>
         <since>
           <model>TI-83+</model>
           <os-version>1.16</os-version>
         </since>
         <lang code="en" ti-ascii="7F">
-          <display>⍯</display>
+          <display>⌸</display>
           <accessible>invertedequal</accessible>
-          <variant>⌸</variant>
         </lang>
       </version>
     </token>
   </two-byte>
   <token value="$BC">
     <version>
       <since>
@@ -9310,14 +9308,38 @@
         </since>
         <lang code="en" ti-ascii="465241432D415050524F58">
           <display>FRAC-APPROX</display>
           <accessible>[FRAC-APPROX]</accessible>
         </lang>
       </version>
     </token>
+    <token value="$3F">
+      <version>
+        <since>
+          <model>TI-84+</model>
+          <os-version>2.55</os-version>
+        </since>
+        <lang code="en" ti-ascii="5354415457495A415244204F4E">
+          <display>STATWIZARD ON</display>
+          <accessible>[STATWIZARD ON]</accessible>
+        </lang>
+      </version>
+    </token>
+    <token value="$40">
+      <version>
+        <since>
+          <model>TI-84+</model>
+          <os-version>2.55</os-version>
+        </since>
+        <lang code="en" ti-ascii="5354415457495A415244204F4646">
+          <display>STATWIZARD OFF</display>
+          <accessible>[STATWIZARD OFF]</accessible>
+        </lang>
+      </version>
+    </token>
     <token value="$41">
       <version>
         <since>
           <model>TI-84+CSE</model>
           <os-version>4.0</os-version>
         </since>
         <lang code="en" ti-ascii="424C5545">
```

### Comparing `tivars-0.8.2/tivars/tokenizer/tokens/scripts/parse.py` & `tivars-0.9.0/tivars/tokens/scripts/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     "TI-82AEP": 60,
 
     "latest": 9999999
 }
 
 
 @functools.total_ordering
-@dataclass
+@dataclass(frozen=True)
 class OsVersion:
     """
     Data class for defining and comparing OS versions
 
-    An OS version is defined by its model and verison number.
+    An OS version is defined by its model and version number.
     The model name must appear in the MODEL_ORDER map above.
     The version number must be of the form "x1.x2.....xn", where each xi is an integer.
 
     Both the model and version can also be empty or "latest".
     An empty model/version is always first in version ordering, while "latest" is always last.
     """
     
@@ -72,22 +72,21 @@
             elif other.version == "latest":
                 return True
             elif other.version == "":
                 return False
             elif self.version == "":
                 return True
             else:
-                return any(map(lambda a: a[0] < a[1],
-                               zip(map(int, self.version.split(".")), map(int, other.version.split(".")))))
+                return self.version.split(".") < other.version.split(".")
 
     def __eq__(self, other):
         return MODEL_ORDER[self.model] == MODEL_ORDER[other.model] and self.version == other.version
 
     @staticmethod
-    def from_element(element) -> 'OsVersion':
+    def from_element(element: ET.Element) -> 'OsVersion':
         """
         Constructs an instance from an XML element in a token sheet
 
         :param element: An XML element
         :return: An OS version corresponding to the element
         """
         
@@ -149,15 +148,15 @@
         """
         :return: A list of all names in this translation used for tokenization
         """
         
         return [self.accessible, *self.variants]
 
     @staticmethod
-    def from_element(element) -> (str, 'Translation'):
+    def from_element(element: ET.Element) -> (str, 'Translation'):
         """
         Constructs an instance and its key from an XML element in a token sheet
 
         :param element: An XML element
         :return: A tuple of a string key and a token translation corresponding to the element
         """
         
@@ -171,27 +170,27 @@
 
         for child in element:
             match child.tag:
                 case "display":
                     display = child.text
                 case "accessible":
                     accessible = child.text
-                case "variants":
+                case "variant":
                     variants.append(child.text)
 
         return code, Translation(ti_ascii, display, accessible, variants)
 
 
 class Token:
     """
     Data class for storing all information about a single token
 
     A token stores the following:
         - The bytes for this token on-calc
-        - The translations of this tokens in all supported languages
+        - The translations of this token in all supported languages
         - The earliest OS version supporting this token
         - The latest OS version supporting this token
         - Any additional attributes stored in the token sheets
     """
     
     def __init__(self, bits: bytes, langs: dict[str, Translation], attrs: dict[str, str] = None,
                  since: OsVersion = OsVersions.INITIAL,
@@ -199,15 +198,15 @@
         self.bits = bits
         self.langs = langs
         self.attrs = attrs
         self.since = since
         self.until = until
 
     @staticmethod
-    def from_element(element, bits, version=OsVersions.LATEST):
+    def from_element(element: ET.Element, bits: bytes, version: OsVersion = OsVersions.LATEST):
         """
         Constructs an instance from an XML element in the token sheets
 
         :param element: An XML element
         :param bits: The token's bytes
         :param version: A minimum OS version (defaults to latest)
         :return: A token corresponding to the element and bits
@@ -235,14 +234,15 @@
                         if until > version_until:
                             until = version_until
 
                     case "lang":
                         if not done:
                             code, translation = Translation.from_element(child)
                             langs[code] = translation
+
         return Token(bits, langs, attrs=element.attrib, since=since, until=until)
 
 
 class Tokens:
     """
     Data class for storing maps between text and tokens
 
@@ -253,42 +253,42 @@
     """
     
     def __init__(self, byte_map: dict[bytes, Token], lang_map: dict[str, dict[str, bytes]]):
         self.bytes = byte_map
         self.langs = lang_map
 
     @staticmethod
-    def from_xml_string(xml_str: str, version=OsVersions.LATEST):
+    def from_xml_string(xml_str: str, version: OsVersion = OsVersions.LATEST):
         """
         Constructs an instance from an XML string
 
         :param xml_str: An XML string
         :param version: A minimum OS version (defaults to latest)
         :return: Token maps corresponding to the string
         """
         
         return Tokens.from_element(ET.fromstring(xml_str), version=version)
 
     @staticmethod
-    def from_element(root, version=OsVersions.LATEST):
+    def from_element(root: ET.Element, version: OsVersion = OsVersions.LATEST):
         """
         Constructs an instance from an XML element in the token sheets
 
         :param root: An XML element, which must be the root element of the sheet
-        :param version: A minimum OS version (defauls to latest)
+        :param version: A minimum OS version (defaults to latest)
         :return: Token maps corresponding to the root element
         """
         
         if root.tag != "tokens":
             raise ValueError("Not a tokens xml.")
 
         all_bytes: dict[bytes, Token] = {}
         all_langs: dict[str, dict[str, bytes]] = {}
 
-        def parse_page(element, bits=b""):
+        def parse_page(element: ET.Element, bits: bytes = b""):
             nonlocal all_bytes
             nonlocal all_langs
 
             if element.tag == "token":
                 token_bits = bits + bytes.fromhex(element.attrib["value"][1:])
                 token = Token.from_element(element, token_bits, version=version)
```

### Comparing `tivars-0.8.2/tivars/tokenizer/tokens/scripts/trie.py` & `tivars-0.9.0/tivars/tokens/scripts/trie.py`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/types/__init__.py` & `tivars-0.9.0/tivars/types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 
 # Makes pydoctor happy
 from typing import TYPE_CHECKING
 
 from .appvar import *
 from .complex import *
+from .flash import *
 from .gdb import *
 from .group import *
 from .list import *
 from .matrix import *
 from .real import *
 from .picture import *
 from .settings import *
 from .tokenized import *
 
+from ..flash import TIFlashHeader, DeviceType
 from ..var import TIEntry
 
 
 if TYPE_CHECKING:
     __all__ = []
 
 else:
-    __all__ = ["TIEntry",
+    __all__ = ["TIEntry", "TIFlashHeader",
                "TIReal",
                "TIRealList", "TIMatrix",
                "TIEquation", "TIString",
                "TIProgram", "TIAsmProgram", "TIProtectedProgram", "TIProtectedAsmProgram",
                "TIPicture", "TIMonoPicture",
                "TIMonoGDB", "TIGDB", "TIGraphedEquation",
                "TIMonoFuncGDB", "TIMonoParamGDB", "TIMonoPolarGDB", "TIMonoSeqGDB",
@@ -40,9 +42,11 @@
                "TIAppVar",
                "TIGroup",
                "TIRealFraction",
                "TIImage",
                "TIComplexFraction",
                "TIRealRadical", "TIComplexRadical",
                "TIComplexPi", "TIComplexPiFraction",
-               "TIRealPi", "TIRealPiFraction"
+               "TIRealPi", "TIRealPiFraction",
+               "TIOperatingSystem", "TIApp", "TICertificate", "TILicense",
+               "DeviceType"
                ]
```

### Comparing `tivars-0.8.2/tivars/types/appvar.py` & `tivars-0.9.0/tivars/types/appvar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Appvars
 """
 
 
 from tivars.models import *
-from ..var import SizedEntry
+from tivars.var import SizedEntry
 
 
 class TIAppVar(SizedEntry, register=True):
     """
     Parser for application variables (appvars)
 
     An appvar is a sized block of data, to be interpreted by the corresponding app as desired.
```

### Comparing `tivars-0.8.2/tivars/types/complex.py` & `tivars-0.9.0/tivars/types/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Complex numeric types
 """
 
 
 from typing import Type
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from ..data import *
-from ..var import TIEntry
-from .numeric import *
+from tivars.numeric import *
+from tivars.var import TIEntry
 from .real import *
 
 
 class RealPart(Converter):
     """
     Converter for the real part of complex numbers
 
@@ -21,15 +21,15 @@
     """
 
     _T = RealEntry
 
     @classmethod
     def get(cls, data: bytes, *, instance=None) -> _T:
         """
-        Converts ``bytes`` -> `RealType`
+        Converts ``bytes`` -> `RealEntry`
 
         :param data: The raw bytes to convert
         :param instance: The instance containing the data section
         :return: The real part of ``data`` converted to the appropriate type
         """
 
         return instance.real_type.get(data)
@@ -56,15 +56,15 @@
     """
 
     _T = RealEntry
 
     @classmethod
     def get(cls, data: bytes, *, instance=None) -> _T:
         """
-        Converts ``bytes`` -> `RealType`
+        Converts ``bytes`` -> `RealEntry`
 
         :param data: The raw bytes to convert
         :param instance: The instance containing the data section
         :return: The real part of ``data`` converted to the appropriate type
         """
 
         return instance.imag_type.get(data)
@@ -219,15 +219,15 @@
 
         return self.get_type(self.imag_subtype_id).real_analogue
 
     def clear(self):
         super().clear()
 
         self.real_subtype_id = 0x0C
-        self.imag_subtype_id = self.type_id
+        self.imag_subtype_id = self._type_id if self._type_id is not None else 0x0C
 
     def components(self) -> (RealEntry, RealEntry):
         """
         :return: The components of this complex number as a pair of `RealEntry` values
         """
 
         return self.real, self.imag
```

### Comparing `tivars-0.8.2/tivars/types/gdb.py` & `tivars-0.9.0/tivars/types/gdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 
 import io
 import json
 import os
 
 from typing import Iterator
-from warnings import warn
+from warnings import catch_warnings, filterwarnings, warn
 
+from tivars.flags import *
+from tivars.data import *
 from tivars.models import *
-from ..flags import *
-from ..data import *
-from ..var import TIEntry, SizedEntry
+from tivars.var import TIEntry, SizedEntry
 from .real import *
 from .tokenized import TIEquation
 
 
 class GraphMode(Flags):
     """
     Flags for GDB graph modes
@@ -64,76 +64,76 @@
 
 
 class GraphStyle(Enum):
     """
     Enum of GDB graph styles
     """
 
-    SolidLine = b'\x00'
-    ThickLine = b'\x01'
-    ShadeAbove = b'\x02'
-    ShadeBelow = b'\x03'
-    Trace = b'\x04'
-    Animate = b'\x05'
-    DottedLine = b'\x06'
+    SolidLine = 0x00
+    ThickLine = 0x01
+    ShadeAbove = 0x02
+    ShadeBelow = 0x03
+    Trace = 0x04
+    Animate = 0x05
+    DottedLine = 0x06
 
     _all = [SolidLine, ThickLine, ShadeAbove, ShadeBelow, Trace, Animate, DottedLine]
     STYLES = _all[:7]
 
 
 class GraphColor(Enum):
     """
     Enum of GDB graph colors
     """
 
-    Mono = b'\x00'
-    Blue = b'\x01'
-    Red = b'\x02'
-    Black = b'\x03'
-    Magenta = b'\x04'
-    Green = b'\x05'
-    Orange = b'\x06'
-    Brown = b'\x07'
-    Navy = b'\x08'
-    LtBlue = b'\x09'
-    Yellow = b'\x0A'
-    White = b'\x0B'
-    LtGray = b'\x0C'
-    MedGray = b'\x0D'
-    Gray = b'\x0E'
-    DarkGray = b'\x0F'
+    Mono = 0x00
+    Blue = 0x01
+    Red = 0x02
+    Black = 0x03
+    Magenta = 0x04
+    Green = 0x05
+    Orange = 0x06
+    Brown = 0x07
+    Navy = 0x08
+    LtBlue = 0x09
+    Yellow = 0x0A
+    White = 0x0B
+    LtGray = 0x0C
+    MedGray = 0x0D
+    Gray = 0x0E
+    DarkGray = 0x0F
 
     _all = [Mono, Blue, Red, Black, Magenta, Green, Orange, Brown, Navy,
             LtBlue, Yellow, White, LtGray, MedGray, Gray, DarkGray]
     COLORS = _all[1:]
 
 
 class GlobalLineStyle(Enum):
     """
     Enum of global GDB line styles
     """
 
-    Thick = b'\x00'
-    DotThick = b'\x01'
-    Thin = b'\x02'
-    DotThin = b'\x03'
+    Thick = 0x00
+    DotThick = 0x01
+    Thin = 0x02
+    DotThin = 0x03
 
     _all = [Thick, Thin, DotThick, DotThin]
     STYLES = _all
 
 
 class BorderColor(Enum):
     """
     Enum of GDB graph border colors
     """
 
-    LtGray = b'\x01'
-    Teal = b'\x02'
-    LtBlue = b'\x03'
-    White = b'\x04'
+    LtGray = 0x01
+    Teal = 0x02
+    LtBlue = 0x03
+    White = 0x04
 
     _all = [LtGray, Teal, LtBlue, White]
     COLORS = _all
 
 
 class EquationFlags(Flags):
     """
@@ -144,15 +144,15 @@
     Deselected = {5: 0}
     UsedForGraph = {6: 1}
     UnusedForGraph = {6: 0}
     LinkTransferSet = {7: 1}
     LinkTransferClear = {7: 0}
 
 
-class TIGraphedEquation(TIEquation):
+class TIGraphedEquation(TIEquation, register=True, override=0x23):
     """
     Parser for equations stored in GDBs
 
     A `TIGraphedEquation` is a `TIEquation` with an extra leading flag byte.
     The equation's style and color in its GDB is bundled for convenience.
     """
 
@@ -171,16 +171,16 @@
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Y1",
                  version: int = None, archived: bool = None,
                  data: bytes = None):
         super().__init__(init, for_flash=for_flash, name=name, version=version, archived=archived, data=data)
 
         self.flags = EquationFlags({0: 1, 1: 1})
-        self.style = b'\x00'
-        self.color = b'\x00'
+        self.style = 0x00
+        self.color = 0x00
 
     def __class_getitem__(cls, index: int):
         index -= 1
 
         class IndexedEquationConverter(Converter):
             """
             Converter for equations within a GDB
@@ -218,24 +218,24 @@
                 # Set appropriate equation
                 equations = list(instance.equations)
                 equations[index] = value
 
                 # Set styles
                 data = instance.raw.calc_data[:instance.offset]
                 for i in range(0, instance.num_equations, instance.num_equations // instance.num_styles):
-                    data += equations[i].style
+                    data += equations[i].raw.style
 
                 # Set data
                 data += b''.join(equation.raw.calc_data for equation in equations)
 
                 # Set colors (if they exist)
                 if color := instance.get_color_data():
                     data += b'84C'
                     for i in range(0, instance.num_equations, instance.num_equations // instance.num_styles):
-                        data += equations[i].color
+                        data += equations[i].raw.color
 
                     data += color[-5:]
 
                 return data
 
         return IndexedEquationConverter
 
@@ -332,22 +332,30 @@
         self.raw.calc_data[1:] = equation.calc_data
 
     def equation(self) -> TIEquation:
         """
         :return: The `TIEquation` component of this GDB equation
         """
 
-        return TIEquation(self.bytes()[:-self.calc_data_length] + self.bytes()[-self.calc_data_length + 1:])
+        # Kinda yucky ngl
+        with catch_warnings():
+            filterwarnings("ignore", "The data section length is incorrect")
+            return TIEquation(self.bytes()[:-self.calc_data_length] + self.bytes()[-self.calc_data_length + 1:])
 
     @Loader[str]
     def load_string(self, string: str, *, model: TIModel = None):
         equation = TIEquation()
         equation.load_string(string, model=model)
         self.load_equation(equation)
 
+    def coerce(self):
+        if self.type_id == 0x23:
+            self.flags |= EquationFlags.Selected
+            self.type_id = 0x03
+
 
 class TIMonoGDB(SizedEntry, register=True):
     """
     Base class for all GDB entries
 
     A GDB is a collection of equations and graph settings representing the state of one of the equation plotters.
     A GDB can correspond to one of the Function, Parametric, Polar, or Sequence plotting modes.
@@ -532,29 +540,29 @@
         data = io.BytesIO(data or self.calc_data[self.offset:])
         equations = tuple(TIGraphedEquation(name=name) for name in self.equation_names)
 
         # Load styles
         for i in range(self.num_styles):
             style = data.read(1)
             for j in range(r := self.num_equations // self.num_styles):
-                equations[r * i + j].style = style
+                equations[r * i + j].raw.style = style
 
         # Load data sections
         for i in range(self.num_equations):
             equations[i].load_data_section(data)
 
         # Load colors (if they exist)
         if rest := data.read():
             data = io.BytesIO(rest)
             data.seek(3, 1)
 
             for i in range(self.num_styles):
                 color = data.read(1)
                 for j in range(r := self.num_equations // self.num_styles):
-                    equations[r * i + j].color = color
+                    equations[r * i + j].raw.color = color
 
         return equations
 
     def get_min_os(self, data: bytes = None) -> OsVersion:
         return max([TIGraphedEquation.get_min_os(eq) for eq in self.get_equations(data)], default=OsVersions.INITIAL)
 
     def get_version(self, data: bytes = None) -> int:
@@ -576,14 +584,15 @@
             'Sequence': 0x80
         }.get(mode := dct.get("graphMode", "Function"), 0x00)
 
         # Load formatSettings
         for setting in dct.get("formatSettings", []):
             try:
                 self.mode_flags |= getattr(GraphMode, setting)
+
             except AttributeError:
                 warn(f"Unrecognized format setting ({setting}).",
                      UserWarning)
 
         # Load extSettings
         ext_settings = dct.get("extSettings", {})
         if "showExpr" in ext_settings:
@@ -768,15 +777,15 @@
 
     def dict(self) -> dict:
         return {
             "global84CSettings": {
                 "colors": {
                     "grid": GraphColor.get_name(self.grid_color),
                     "axes": GraphColor.get_name(self.axes_color),
-                    "border": self.border_color[0]
+                    "border": self.border_color
                 },
                 "other": {
                     "globalLineStyle": GlobalLineStyle.get_name(self.global_line_style),
                     "detectAsymptotes": GraphMode.DetectAsymptotesOn in self.color_mode_flags
                 }
             }
         }
@@ -1428,14 +1437,15 @@
                     self.extended_mode_flags |= GraphMode.SEQ_np1
                 case "SEQ(n+2)":
                     self.extended_mode_flags |= GraphMode.SEQ_np2
 
         if "seqSettings" in dct:
             try:
                 self.sequence_flags |= getattr(SeqMode, dct["seqMode"])
+
             except AttributeError:
                 warn(f"Unrecognized sequence mode ({dct['seqMode']}).",
                      UserWarning)
 
     def dict(self) -> dict:
         dct = super().dict()
```

### Comparing `tivars-0.8.2/tivars/types/group.py` & `tivars-0.9.0/tivars/types/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 
 import io
 
 from typing import Sequence
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from ..data import *
-from ..var import TIEntry, SizedEntry
+from tivars.var import TIEntry, SizedEntry
 from .gdb import TIGraphedEquation
 
 
 class TIGroup(SizedEntry, register=True):
     """
     Parser for group objects
 
@@ -61,26 +61,26 @@
         group = TIGroup(for_flash=entries[0].meta_length > TIEntry.base_meta_length, name=name)
 
         for index, entry in enumerate(entries):
             name = entry.raw.name.rstrip(b'\x00')
             vat = bytearray([entry.type_id, 0, entry.version, 0, 0, entry.archived])
 
             if entry.archived:
-                warn(f"Entry #{index} is archived, which may lead to unexpected behavior on-calc.",
+                warn(f"Entry #{index} ({type(entry)}) is archived, which may lead to unexpected behavior on-calc.",
                      UserWarning)
 
             if isinstance(entry, TIGraphedEquation):
                 vat[0] |= entry.raw.flags
 
             match entry.type_id:
                 case 0x05 | 0x06 | 0x15 | 0x17:
-                    vat += [len(name), *name]
+                    vat += bytearray([len(name), *name])
 
                 case 0x01 | 0x0D:
-                    vat += [len(name) + 1, *name, 0]
+                    vat += bytearray([len(name) + 1, *name, 0])
 
                 case _:
                     vat += name.ljust(3, b'\x00')
 
             group.data += vat
             group.data += entry.calc_data
 
@@ -109,15 +109,15 @@
         data = io.BytesIO(data or self.data[:])
         entries = []
 
         index = 1
         while type_byte := data.read(1):
             _, version = data.read(2)
 
-            match type_id := type_byte[0] & 15:
+            match type_id := type_byte[0] & 63:
                 case 0x05 | 0x06 | 0x15 | 0x17:
                     *_, page, length = data.read(4)
 
                     if length > 8:
                         warn(f"The name length of entry #{index} ({length}) exceeds eight.",
                              BytesWarning)
```

### Comparing `tivars-0.8.2/tivars/types/json/func.default.json` & `tivars-0.9.0/tivars/types/json/func.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/types/json/param.default.json` & `tivars-0.9.0/tivars/types/json/param.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/types/json/polar.default.json` & `tivars-0.9.0/tivars/types/json/polar.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/types/json/seq.default.json` & `tivars-0.9.0/tivars/types/json/seq.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.8.2/tivars/types/list.py` & `tivars-0.9.0/tivars/types/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Lists
 """
 
 
 import re
 
 from io import BytesIO
-from typing import ByteString, Iterator, Sequence
+from typing import Iterator, Sequence
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from tivars.tokenizer import TokenizedString
-from ..data import *
-from ..var import TIEntry
+from tivars.tokenizer import *
+from tivars.var import TIEntry
 from .complex import ComplexEntry
 from .real import RealEntry
 
 
 class ListName(TokenizedString):
     """
     Converter for the name section of lists
@@ -84,15 +84,15 @@
     versions = [0x10, 0x0B, 0x00]
 
     min_data_length = 2
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "L1",
                  version: int = None, archived: bool = None,
-                 data: ByteString = None):
+                 data: bytes = None):
 
         super().__init__(init, for_flash=for_flash, name=name, version=version, archived=archived, data=data)
 
     def __format__(self, format_spec: str) -> str:
         match format_spec:
             case "":
                 return "[" + ", ".join(format(entry, format_spec) for entry in self.list()) + "]"
@@ -152,15 +152,15 @@
 
         else:
             return 0x00
 
     def supported_by(self, model: TIModel) -> bool:
         return super().supported_by(model) and (self.get_version() <= 0x0B or model.has(TIFeature.ExactMath))
 
-    @Loader[ByteString, BytesIO]
+    @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         super().load_bytes(data)
 
         if self.calc_data_length // self._E.min_data_length != self.length:
             warn(f"The list has an unexpected length "
                  f"(expected {self.calc_data_length // self._E.min_data_length}, got {self.length}).",
                  BytesWarning)
```

### Comparing `tivars-0.8.2/tivars/types/matrix.py` & `tivars-0.9.0/tivars/types/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Matrices
 """
 
 
 from io import BytesIO
-from typing import ByteString, Iterator, Sequence
+from typing import Iterator, Sequence
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from ..data import *
-from ..var import TIEntry
+from tivars.var import TIEntry
 from .real import RealEntry
 
 
 class TIMatrix(TIEntry, register=True):
     """
     Parser for the matrix type
 
@@ -128,15 +128,15 @@
 
         else:
             return 0x00
 
     def supported_by(self, model: TIModel) -> bool:
         return super().supported_by(model) and (self.get_version() <= 0x0B or model.has(TIFeature.ExactMath))
 
-    @Loader[ByteString, BytesIO]
+    @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         super().load_bytes(data)
 
         if self.calc_data_length // RealEntry.min_data_length != self.size:
             warn(f"The matrix has an unexpected size "
                  f"(expected {self.calc_data_length // RealEntry.min_data_length}, got {self.size}).",
                  BytesWarning)
```

### Comparing `tivars-0.8.2/tivars/types/numeric.py` & `tivars-0.9.0/tivars/numeric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Numeric helper functions and converters
 """
 
 
 import decimal as dec
 
-from ..data import *
+from .data import *
 
 
 with dec.localcontext() as ctx:
     ctx.prec = 16
     pi, prev = 3, 0
     t = dec.Decimal(3)
 
@@ -85,23 +85,24 @@
             value *= 100
             tens, ones = divmod(byte, 16)
             value += 10 * tens + ones
 
         return value
 
     @classmethod
-    def set(cls, value: _T, **kwargs) -> bytes:
+    def set(cls, value: _T, *, length: int = None, **kwargs) -> bytes:
         """
         Converts ``int`` -> ``bytes`` as 2-digit binary coded decimal
 
         :param value: The value to convert
+        :param length: The length of the data section
         :return: The bytes representing ``value`` in BCD
         """
 
-        return int.to_bytes(int(str(value), 16), 7, 'big')
+        return int.to_bytes(int(str(value), 16), length if length is not None else 7, 'big')
 
 
 class LeftNibbleBCD(Converter):
     """
     Converter for 2-digit binary-coded decimal with a single extra nibble
 
     A single byte contains two decimal digits as if they were hex digits.
@@ -124,15 +125,15 @@
             value *= 100
             tens, ones = divmod(byte, 16)
             value += 10 * tens + ones
 
         return value
 
     @classmethod
-    def set(cls, value: _T, current: bytes = None, **kwargs) -> bytes:
+    def set(cls, value: _T, *, current: bytes = None, **kwargs) -> bytes:
         """
         Converts ``int`` -> ``bytes`` as 2-digit binary coded decimal with an extra nibble on the left
 
         :param value: The value to convert
         :param current: The current value of the data section
         :return: The bytes representing ``value`` in BCD
         """
@@ -167,15 +168,15 @@
             value *= 100
             tens, ones = divmod(byte, 16)
             value += 10 * tens + ones
 
         return 10 * value + data[-1] // 16
 
     @classmethod
-    def set(cls, value: _T, current: bytes = None, **kwargs) -> bytes:
+    def set(cls, value: _T, *, current: bytes = None, **kwargs) -> bytes:
         """
         Converts ``int`` -> ``bytes`` as 2-digit binary coded decimal with an extra nibble on the right
 
         :param value: The value to convert
         :param current: The current value of the data section
         :return: The bytes representing ``value`` in BCD
         """
```

### Comparing `tivars-0.8.2/tivars/types/picture.py` & `tivars-0.9.0/tivars/types/picture.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Pictures and images
 """
 
 
 from typing import Iterator, Sequence
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
 from tivars.tokenizer import TokenizedString
-from ..data import *
-from ..var import SizedEntry
+from tivars.var import SizedEntry
 
 RGB = tuple[int, int, int]
 
 
 class L1(Converter):
     """
     Converter for black-and-white pixels packed eight-per-byte
```

### Comparing `tivars-0.8.2/tivars/types/real.py` & `tivars-0.9.0/tivars/types/real.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import decimal as dec
 import fractions as frac
 import re
 
 from typing import Type
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from ..data import *
-from ..var import TIEntry
-from .numeric import *
+from tivars.numeric import *
+from tivars.var import TIEntry
 
 
 class RealEntry(TIEntry):
     """
     Base class for real numeric types
 
     This class handles floating-point types as well as the exact formats for the TI-83PCE and other newer models.
```

### Comparing `tivars-0.8.2/tivars/types/settings.py` & `tivars-0.9.0/tivars/types/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 
 import json
 
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
-from ..data import *
-from ..var import SizedEntry
+from tivars.var import SizedEntry
 from .real import GraphRealEntry
 
 
 class SettingsEntry(SizedEntry):
     """
     Base class for settings entries
```

### Comparing `tivars-0.8.2/tivars/types/tokenized.py` & `tivars-0.9.0/tivars/types/tokenized.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 Tokenized types
 """
 
 
 import re
 
 from io import BytesIO
-from typing import ByteString
 from warnings import warn
 
+from tivars.data import *
 from tivars.models import *
 from tivars.tokenizer import *
-from ..data import *
-from ..var import SizedEntry
+from tivars.var import SizedEntry
 
 
 class TokenizedEntry(SizedEntry):
     """
     Base class for all tokenized entries
 
     A tokenized entry is a `SizedEntry` whose data comprises a stream of tokens.
@@ -129,15 +128,15 @@
                 version = 0x00
 
         if any(token in (data or self.data) for token in self.clock_tokens):
             version += 0x20
 
         return version
 
-    @Loader[ByteString, BytesIO]
+    @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         super().load_bytes(data)
 
         try:
             if self.version != (version := self.get_version()):
                 warn(f"The version is incorrect (expected 0x{version:02x}, got 0x{self.version:02x}).",
                      BytesWarning)
@@ -267,14 +266,28 @@
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Str1",
                  version: int = None, archived: bool = None,
                  data: bytes = None):
 
         super().__init__(init, for_flash=for_flash, name=name, version=version, archived=archived, data=data)
 
+    @Section(8, TokenizedString)
+    def name(self, value) -> str:
+        """
+        The name of the entry
+
+        Must be one of the string names: ``Str1`` - ``Str0``
+        """
+
+        if not re.fullmatch(r"Str\d", varname := value[:4].capitalize()):
+            warn(f"String has an invalid name: {varname}.",
+                 BytesWarning)
+
+        return varname
+
     @Loader[str]
     def load_string(self, string: str, *, model: TIModel = None):
         super().load_string(string.strip("\"'"))
 
     def string(self) -> str:
         return f"\"{super().string()}\""
 
@@ -323,15 +336,15 @@
         """
 
         varname = value[:8].upper()
         varname = re.sub(r"(\u03b8|\u0398|\u03F4|\u1DBF)", "θ", varname)
         varname = re.sub(r"[^θa-zA-Z0-9]", "", varname)
 
         if not varname or varname[0].isnumeric():
-            warn(f"Var has invalid name: {varname}.",
+            warn(f"Program has an invalid name: {varname}.",
                  BytesWarning)
 
         return varname
 
     def protect(self):
         """
         Cast this program to a protected program
@@ -344,30 +357,56 @@
         """
         Cast this program to an unprotected program
         """
 
         self.type_id = 0x05
         self.coerce()
 
-    @Loader[ByteString, BytesIO]
+    @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         super(TokenizedEntry, self).load_bytes(data)
 
         try:
             if self.version != (version := self.get_version()):
                 warn(f"The version is incorrect (expected 0x{version:02x}, got 0x{self.version:02x}).",
                      BytesWarning)
 
         except ValueError as e:
             if self.is_tokenized:
                 warn(f"The file contains an invalid token {' '.join(str(e).split()[2:])}.",
                      BytesWarning)
 
+    @Loader[str]
+    def load_string(self, string: str, *, model: TIModel = None, lang: str = None):
+        super().load_string(string, model=model, lang=lang)
+
+        if not self.is_tokenized:
+            warn("ASM programs may not have tokenized data.",
+                 UserWarning)
+
+    def string(self) -> str:
+        string = super().string()
+
+        if not self.is_tokenized:
+            warn("ASM programs may not have tokenized data.",
+                 UserWarning)
+
+        return string
+
     def coerce(self):
-        match self.type_id, any(token in self.data for token in self.asm_tokens):
+        try:
+            self.string()
+            doors = False
+
+        except ValueError:
+            doors = True
+
+        doors &= b"\xEF\x68" in self.data and self.data.index(b"\xEF\x68") > 0
+
+        match self.type_id, any(token in self.data for token in self.asm_tokens) | doors:
             case 0x05, False:
                 self.__class__ = TIProgram
             case 0x05, True:
                 self.__class__ = TIAsmProgram
             case 0x06, False:
                 self.__class__ = TIProtectedProgram
             case 0x06, True:
@@ -401,18 +440,14 @@
         except TypeError:
             return super().__format__(format_spec)
 
     def get_min_os(self, data: bytes = None) -> OsVersion:
         return max([model.OS() for token, model in self.asm_tokens.items() if token in (data or self.data)],
                    default=OsVersions.INITIAL)
 
-    @Loader[str]
-    def load_string(self, string: str, *, model: TIModel = None, lang: str = None):
-        raise NotImplementedError
-
 
 class TIProtectedProgram(TIProgram, register=True):
     """
     Parser for protected programs
 
     A `TIProtectedProgram` is a `TIProgram` with protection against editing.
     """
```

### Comparing `tivars-0.8.2/tivars/var.py` & `tivars-0.9.0/tivars/var.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 The fundamental var components
 """
 
 
 from io import BytesIO
-from typing import BinaryIO, ByteString, Iterator, Type
+from typing import BinaryIO, Iterator, Type
 from warnings import warn
 
-from tivars.models import *
-from tivars.tokenizer import TokenizedString
 from .data import *
+from .models import *
+from .tokenizer import TokenizedString
 
 
 class TIHeader:
     """
     Parser for var file headers
 
     All var files require a header which includes a number of magic bytes, data lengths, and a customizable comment.
@@ -37,23 +37,23 @@
             :return: The bytes contained in this header
             """
 
             return self.magic + self.extra + self.product_id + self.comment
 
     def __init__(self, model: TIModel = None, *,
                  magic: str = None, extra: bytes = b'\x1a\x0a', product_id: int = None,
-                 comment: str = "Created with tivars_lib_py v0.8.2",
+                 comment: str = "Created with tivars_lib_py v0.9.0",
                  data: bytes = None):
         """
         Creates an empty header which targets a specified model
 
         :param model: A minimum `TIModel` to target (defaults to ``TI_83P``)
         :param magic: File magic at the start of the header (default to the model's magic)
-        :param extra: Extra export bytes for the header (defaults to ``0x1a0a``)
-        :param product_id: The targeted model's product ID (defaults to ``0x00``)
+        :param extra: Extra export bytes for the header (defaults to ``$1a0a``)
+        :param product_id: The targeted model's product ID (defaults to ``$00``)
         :param comment: A comment to include in the header (defaults to a simple lib message)
         :param data: This header's data (defaults to empty)
         """
 
         self.raw = self.Raw()
 
         model = model or TI_83P
@@ -175,18 +175,18 @@
     def load_bytes(self, data: bytes | BytesIO):
         """
         Loads a byte string or bytestream into the header
 
         :param data: The source bytes
         """
 
-        try:
+        if hasattr(data, "read"):
             data = BytesIO(data.read())
 
-        except AttributeError:
+        else:
             data = BytesIO(data)
 
         # Read magic
         self.raw.magic = data.read(8)
 
         # Read export bytes
         self.raw.extra = data.read(2)
@@ -322,20 +322,20 @@
                  version: int = None, archived: bool = None,
                  data: bytes = None):
         """
         Creates an empty entry with specified meta and data values
 
         The entry ``version`` and ``archived`` flag are invalid if ``for_flash == False``.
 
-        :param init: Values to initialize this entry's data (defaults to ``None``)
-        :param for_flash: Whether this entry supports flash chips (defaults to ``True``)
-        :param name: The name of this entry (defaults to a valid default name)
-        :param version: This entry's version (defaults to ``None``)
-        :param archived: Whether this entry is archived (defaults to entry's default state on-calc)
-        :param data: This entry's data (defaults to empty)
+        :param init: Values to initialize the entry's data (defaults to ``None``)
+        :param for_flash: Whether the entry supports flash chips (defaults to ``True``)
+        :param name: The name of the entry (defaults to a valid default name)
+        :param version: The entry's version (defaults to ``None``)
+        :param archived: Whether the entry is archived (defaults to entry's default state on-calc)
+        :param data: The entry's data (defaults to empty)
         """
 
         self.raw = self.Raw()
 
         self.meta_length = TIEntry.flash_meta_length if for_flash else TIEntry.base_meta_length
         self.type_id = self._type_id if self._type_id is not None else 0xFF
         self.name = name
@@ -352,17 +352,18 @@
 
         self.clear()
         if data:
             self.data = bytearray(data)
             self.coerce()
 
         elif init is not None:
-            try:
+            if hasattr(init, "bytes"):
                 self.load_bytes(init.bytes())
-            except AttributeError:
+
+            else:
                 self.load(init)
 
         self.version = self.get_version()
 
     def __bool__(self) -> bool:
         """
         :return: Whether this entry's data is empty
@@ -406,19 +407,19 @@
 
         :param format_spec: The format parameters
         :return: A string representation of this entry
         """
 
         raise TypeError(f"unsupported format string passed to {type(self)}.__format__")
 
-    def __init_subclass__(cls, /, register=False, **kwargs):
+    def __init_subclass__(cls, /, register=False, override=None, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if register:
-            TIEntry.register(cls)
+            TIEntry.register(cls, override)
 
     def __iter__(self) -> Iterator:
         """
         :return: If this entry is a container or collection, an iterator over its elements
         """
 
         raise NotImplementedError
@@ -567,22 +568,23 @@
         meta_length = int.from_bytes(stream.read(2), 'little')
         data_length = int.from_bytes(stream.read(2), 'little')
         stream.seek(-4, 1)
 
         return 2 + meta_length + 2 + data_length
 
     @classmethod
-    def register(cls, var_type: type['TIEntry']):
+    def register(cls, var_type: Type['TIEntry'], override: int = None):
         """
         Registers a subtype with this class for coercion
 
         :param var_type: The `TIEntry` subtype to register
+        :param override: A type ID to use for registry that differs from that of the var type
         """
 
-        cls._type_ids[var_type._type_id] = var_type
+        cls._type_ids[var_type._type_id if override is None else override] = var_type
 
     def archive(self):
         """
         Archives this entry (if supported)
         """
 
         if self.flash_bytes:
@@ -637,26 +639,26 @@
         """
 
         if self.flash_bytes:
             self.archived = False
         else:
             raise TypeError("entry does not support archiving.")
 
-    @Loader[ByteString, BytesIO]
+    @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         """
         Loads a byte string or bytestream into this entry
 
         :param data: The bytes to load
         """
 
-        try:
+        if hasattr(data, "read"):
             data = BytesIO(data.read())
 
-        except AttributeError:
+        else:
             data = BytesIO(data)
 
         # Read meta length
         self.raw.meta_length = data.read(2)
 
         # Read data length
         data_length = data.read(2)
@@ -709,15 +711,19 @@
         # Read data and check length
         data_length2 = data.read(2)
         if data_length != data_length2:
             warn(f"The var entry data lengths are mismatched ({data_length} vs. {data_length2}); "
                  f"using {data_length2} to read the data section.",
                  BytesWarning)
 
-        self.raw.calc_data = bytearray(data.read(int.from_bytes(data_length2, 'little')))
+        self.raw.calc_data = bytearray(data.read(length := int.from_bytes(data_length2, 'little')))
+
+        if len(self.calc_data) != length:
+            warn(f"The data section length is incorrect (expected {length}, got {len(self.calc_data)}).",
+                 BytesWarning)
 
         self.coerce()
 
         if self.versions != [0x00] and self.version not in self.versions:
             warn(f"The version (0x{self.version:02x}) is not recognized.",
                  BytesWarning)
 
@@ -799,27 +805,28 @@
         :param filename: A filename to open
         :return: The (first) entry stored in the file
         """
 
         if cls._type_id is not None and \
                 not any(filename.endswith(extension) for extension in cls.extensions.values()):
             warn(f"File extension .{filename.split('.')[-1]} not recognized for var type {cls}; "
-                 f"attempting to read anyway.")
+                 f"attempting to read anyway.",
+                 UserWarning)
 
         with open(filename, 'rb') as file:
             file.seek(55)
 
             entry = cls()
             entry.load_bytes(file.read(cls.next_entry_length(file)))
 
             file.seek(2, 1)
 
             if file.read():
                 warn("The selected var file contains multiple entries; only the first will be loaded. "
-                     "Use load_from_file to select a particular entry, or load the entire file in a TIVar object.",
+                     "Use load_from_file to select a particular entry, or load the entire file into a TIVar object.",
                      UserWarning)
 
         return entry
 
     def save(self, filename: str = None, *, header: TIHeader = None, model: TIModel = None):
         """
         Saves this entry as a var file given a filename and optional header and targeted model
@@ -856,14 +863,18 @@
                 self.__class__ = subclass
                 self.coerce()
 
             elif self.type_id != 0xFF:
                 warn(f"Type ID 0x{self.type_id:02x} is not recognized; entry will not be coerced to a subclass.",
                      BytesWarning)
 
+            else:
+                warn("Type ID is 0xFF; no coercion will occur.",
+                     UserWarning)
+
 
 class TIVar:
     """
     Container for var files
 
     A var file is composed of a header and any number of entries (though most have only one).
     """
@@ -871,15 +882,15 @@
     def __init__(self, *, name: str = "UNNAMED", header: TIHeader = None, model: TIModel = None, data: bytes = None):
         """
         Creates an empty var with a specified name, header, and targeted model
 
         :param name: The name of the var (defaults to ``UNNAMED``)
         :param header: A `TIHeader` to attach (defaults to an empty header)
         :param model: A minimum `TIModel` to target (defaults to ``None``)
-        :param data: This var's data (defaults to empty)
+        :param data: The var's data (defaults to empty)
         """
 
         self._header = header or TIHeader(model)
         self.entries = []
 
         self.name = name
         self._model = model
@@ -943,27 +954,27 @@
 
         This should always be 57 less than the total var size.
         """
 
         return sum(len(entry) for entry in self.entries)
 
     @property
-    def checksum(self):
+    def checksum(self) -> bytes:
         """
         The checksum for the var
 
         This is equal to the lower 2 bytes of the sum of all bytes in the entries.
         """
 
         return int.to_bytes(sum(sum(entry.bytes()) for entry in self.entries) & 0xFFFF, 2, 'little')
 
     @property
     def extension(self) -> str:
         """
-        Determines the var's file extension based on its entries and targeted model.
+        Determines the var's file extension based on its entries and targeted model
 
         If there is only one entry, that entry's extension for the target model is used.
         Otherwise, ``.8xg`` is used.
 
         :return: The var's file extension
         """
 
@@ -990,15 +1001,15 @@
 
         except IndexError:
             raise ValueError("this var is empty")
 
     @property
     def filename(self) -> str:
         """
-        Determines the var's filename based on its name, entries, and targeted model.
+        Determines the var's filename based on its name, entries, and targeted model
 
         The filename is the concatenation of the var name and extension (see `TIVar.extension`).
 
         :return: The var's filename
         """
 
         return f"{self.name}.{self.extension}"
@@ -1069,34 +1080,44 @@
     def load_bytes(self, data: bytes | BytesIO):
         """
         Loads a byte string or bytestream into this var
 
         :param data: The bytes to load
         """
 
-        try:
+        if hasattr(data, "read"):
             data = BytesIO(data.read())
 
-        except AttributeError:
+        else:
             data = BytesIO(data)
 
         # Read header
         self._header.load_bytes(data.read(53))
         entry_length = int.from_bytes(data.read(2), 'little')
 
         # Read entries
         self.clear()
-        while entry_length:
+        while entry_length > 0:
             self.add_entry()
 
             length = TIEntry.next_entry_length(data)
-            self.entries[-1].load_bytes(data.read(length))
+            self.entries[-1].load_bytes(entry_data := data.read(length))
+
+            if len(entry_data) != length:
+                warn(f"The data length of entry #{len(self.entries) - 1} ({type(self.entries[-1])}) is incorrect "
+                     f"(expected {length}, got {len(entry_data)}).",
+                     BytesWarning)
 
             entry_length -= length
 
+        if entry_length < 0:
+            warn(f"The total length of entries is incorrect (expected {self.entry_length + entry_length}, "
+                 f"got {self.entry_length}).",
+                 BytesWarning)
+
         # Read checksum
         checksum = data.read(2)
 
         # Check model
         if self._model and not self._model <= min(*self._header.targets()):
             warn(f"The loaded var file is incompatible with the {self._model}.",
                  BytesWarning)
@@ -1183,15 +1204,16 @@
         pass
 
     def clear(self):
         self.raw.calc_data = bytearray([0, 0, *self.leading_bytes])
         self.raw.calc_data.extend(bytearray(self.min_data_length - self.calc_data_length))
         self.length = len(self.leading_bytes) + len(self.data)
 
-    def load_bytes(self, data: ByteString):
+    @Loader[bytes, bytearray, BytesIO]
+    def load_bytes(self, data: bytes | BytesIO):
         super().load_bytes(data)
 
         if self.length != (data_length := len(self.leading_bytes) + len(self.data)):
             warn(f"The entry has an unexpected data length (expected {self.length}, got {data_length}).",
                  BytesWarning)
 
     def load_data_section(self, data: BytesIO):
```

### Comparing `tivars-0.8.2/tivars.egg-info/PKG-INFO` & `tivars-0.9.0/tivars.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tivars
-Version: 0.8.2
+Version: 0.9.0
 Summary: A library for interacting with TI-(e)z80 (82/83/84 series) calculator files
 License: The MIT License (MIT)
         
         Copyright (c) 2023 kg583
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,107 +35,109 @@
 Provides-Extra: arrays
 Requires-Dist: numpy; extra == "arrays"
 
 # tivars_lib_py
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
-Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting).
+Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.8.2`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
 
 Alternatively, you can clone this repository or [download a release](https://github.com/TI-Toolkit/tivars_lib_py/tags) and extract the `tivars` directory to include it in your next project. Once downloaded, you can also use `pip` to install it locally.
 
 ### As a Submodule
 
-Include this repository in your next project as a submodule using `git submodule` or manually cloning and writing the following in `.gitmodules`:
-
-```
-[submodule "tivars_lib_py"]
-	path = path/to/tivars_lib_py
-	url = https://github.com/TI-Toolkit/tivars_lib_py.git
-```
-
-Then, add the following to any file which imports `tivars`:
+Include this repository in your next project as a submodule using the `git submodule` command. Then, add the following to any file which imports `tivars`:
 
 ```py
 import sys
 
 sys.path.insert(1, 'tivars_lib_py/')
 ```
 
 Check out [this tool](https://github.com/TI-Toolkit/token_translation_extractor) for an example.
 
 ### Unit Testing
 
 You can run the test suite via `__main__.py`, or run individual tests found in `tests/` with `unittest`. Tests for optional package extensions (e.g. PIL) will be skipped if the package cannot be found.
 
-Note that the PyPI distribution does _not_ include the test suite.
+> [!WARNING]
+> The PyPI distribution does _not_ include the test suite.
 
 ## How to Use
 
-### Creating vars
+### Creating objects
+
+### Var basics
 
 Every var file has two parts: a _header_ and a number of _entries_, where an entry contains the data for a single variable. Usually, var files contain just one entry; in these cases, there's not much distinction between a var and an entry for the purposes of messing with its data.
 
+### Entries
+
 To create an empty entry, instantiate its corresponding type from `tivars.types`. You can specify additional parameters as you like:
 
 ```python
 from tivars.models import *
 from tivars.types import *
 
 my_program = TIProgram(name="HELLO")
 ```
 
-If you're not sure of an entry's type, instantiate a base `TIEntry`:
+> [!TIP]
+> If you're not sure of an entry's type, you can instantiate a base `TIEntry`.
 
-```python
-my_entry = TIEntry()
-```
+### Vars and Headers
 
 If you want to create an entire var or just a header, use `TIVar` or `TIHeader` instead:
 
 ```python
 from tivars.var import *
 
 my_var = TIVar()
 my_var_for84pce = TIVar(model=TI_84PCE)
 
 my_header = TIHeader()
 my_header_with_a_cool_comment = TIHeader(comment="Wow! I'm a comment!")
 ```
 
-### Reading and writing
+### Reading files
+
+#### Vars
 
 Vars can be loaded from files or raw bytes:
 
 ```python
 my_var = TIVar.open("HELLO.8xp")
 
-# Note binary mode!
 with open("HELLO.8xp", 'rb') as file:
     my_var.load_var_file(file)
     
     file.seek(0)
     my_var.load_bytes(file.read())
 ```
 
+> [!IMPORTANT]
+> When loading from a file object, make sure the file is opened in binary mode.
+
+#### Entries
+
 Entries can be loaded from files or raw bytes. When loading from a file, you may specify which entry to load if there are multiple:
 
 ```python
-# Raises an error if the var has multiple entries; use load_from_file instead
+# Raises an error if the var has multiple entries
 my_program = TIProgram.open("HELLO.8xp")
 
 with open("HELLO.8xp", 'rb') as file:
     # Offset counts the number of entries to skip; defaults to zero
     my_program.load_from_file(file, offset=1)
     
     file.seek(0)
@@ -149,32 +151,46 @@
 my_program.load_string("Disp \"HELLO WORLD!\"")
 
 my_real = TIReal(1.23)
 my_real.load_float(1.23)
 ```
 
 Base `TIEntry` objects, as well other parent types like `TIGDB`, will be automatically coerced to the correct type:
+
 ```python
 # Coerces to a TIProgram
 my_entry = TIEntry.open("HELLO.8xp")
 ```
 
+> [!TIP]
+> Any entry type can be cast to any other by setting the object's `__class__`.
+
+### Exporting objects
+
+#### Vars
+
 Export a var as bytes or straight to a file:
 
 ```python
 my_var.save("HELLO.8xp")
 
 # Infer the filename and extension
 my_var.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_var.bytes())
 ```
 
+> [!IMPORTANT]
+> `.save()` uses the var's name as the filename, saving to the current working directory.
+
+#### Entries
+
 Entries can be passed an explicit header to attach or model to target when exporting:
+
 ```python
 my_program.save("HELLO.8xp")
 my_program.save()
 
 with open("HELLO.8xp", 'wb+') as file:
     file.write(my_program.export(header=my_header).bytes())
 ```
@@ -183,23 +199,20 @@
 
 ```python
 assert my_program.string() == "Disp \"HELLO WORLD!\""
 
 assert my_real.float() == 1.23
 ```
 
-Data types corresponding to built-in Python types can be obtained from the built-in constructors:
-
-```python
-assert str(my_program) == "Disp \"HELLO WORLD!\""
+> [!TIP]
+> Built-in types can be exported to using the standard constructors, e.g. `str(my_program)`.
 
-assert float(my_real) == 1.23
-```
+### Data Manipulation
 
-### Data Sections
+#### Data sections
 
 Vars are comprised of individual _sections_ which represent different forms of data, split across the header and entries. The var itself also contains the total entry length and checksum sections, but these are read-only to prevent file corruption.
 
 You can read and write to individual sections of an entry or header as their "canonical" type:
 
 ```python
 my_header.comment = "This is my (even cooler) comment!"
@@ -215,19 +228,41 @@
 my_gdb.Xmin = TIReal(0)
 
 assert my_gdb.Xmax == TIReal(10)
 ```
 
 Each section is annotated with the expected type.
 
+> [!TIP]
+> Data sections can accept any subtype of their expected type.
+
+#### Raw containers
+
+All vars store their data sections as raw bytes in the format interpreted by the calculator. Access any data section as a member of the `.raw` attribute to view and edit these bytes directly.
+
+```python
+my_header.raw.comment = "This is my (even rawer) comment!".encode('utf-8')
+my_program.raw.archived = b'\x80'
+
+assert my_program.raw.type_id == b'\x05'
+```
+
+> [!WARNING]
+> Edits to read-only bytes like the checksum are reset whenever any other data in the var is updated.
+
 ### Models
 
 All TI-82/83/84 series calcs are represented as `TIModel` objects stored in `tivars.models`. Each model contains its name, metadata, and features; use `has` on a `TIFeature` to check that a model has a given a feature. Models are also used to determine var file extensions and token sheets.
 
-For these reasons, it is _not_ recommended to instantiate your own models.
+### Flash Files
+
+Flash files such as apps, OSes, and certificates can be loaded using the `TIFlashHeader` base class or its children. A flash file is composed of one to three headers (though usually only one); these are not to be confused with var headers. A flash header does _not_ need to be "packaged" into a larger file format like an entry in a regular var; see `TIFlashHeader.open` and `TIFlashHeader.save`.
+
+> [!TIP]
+> Loading flash files into a `TIEntry` probably won't work very well.
 
 ## Other Functionalities
 
 ### PIL
 
 The `tivars.PIL` package can be used to interface with PIL, the Python Imaging Library. Simply import the package to register codecs for each of the TI image types. You can then open such images directly into a PIL `Image`:
 
@@ -237,18 +272,24 @@
 
 img = Image.open("Pic1.8ci")
 img.show()
 ```
 
 ### Tokenization
 
-Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. Support currently exists for all models in the 82/83/84 series as well as the TI-73; PR's concerning the sheets themselves should be directed upstream to [TI-Toolkit/tokens](https://github.com/TI-Toolkit/tokens).
+Functions to decode and encode strings into tokens can be found in `tivars.tokenizer`. These functions utilize the [TI-Toolkit token sheets](https://github.com/TI-Toolkit/tokens), which are kept as a submodule in `tivars.tokens`. Support currently exists for all models in the 82/83/84 series; PR's concerning the sheets themselves should be directed upstream.
+
+> [!IMPORTANT]
+> In contrast to some other tokenizers like SourceCoder, tokenization does _not_ depend on whether the content appears inside a BASIC string literal. Text is always assigned to the _longest_ permissible token.
 
 ## Documentation
 
 Library documentation can be found on [GitHub Pages](https://ti-toolkit.github.io/tivars_lib_py/).
 
 The var file format(s) and data sections can be found in a readable format on the [repository wiki](https://github.com/TI-Toolkit/tivars_lib_py/wiki). Much of the information is copied from the [TI-83 Link Guide](http://merthsoft.com/linkguide/ti83+/vars.html), though has been updated to account for color models.
 
+> [!NOTE]
+> The wiki is still a work-in-progress. Why not [contribute a page](https://github.com/TI-Toolkit/tivars_lib_py/wiki)?
+
 ## Examples
 
 You can find more sample code in `examples` that details common operations on each of the entry types. There are also examples for interfacing with popular external libraries (e.g. NumPy, PIL). Contributions welcome!
```

### Comparing `tivars-0.8.2/tivars.egg-info/SOURCES.txt` & `tivars-0.9.0/tivars.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 tivars/__init__.py
 tivars/data.py
 tivars/flags.py
+tivars/flash.py
+tivars/numeric.py
 tivars/var.py
 tivars.egg-info/PKG-INFO
 tivars.egg-info/SOURCES.txt
 tivars.egg-info/dependency_links.txt
 tivars.egg-info/requires.txt
 tivars.egg-info/top_level.txt
 tivars/PIL/TI8caPlugin.py
@@ -15,27 +17,30 @@
 tivars/PIL/TI8xiPlugin.py
 tivars/PIL/__init__.py
 tivars/PIL/common.py
 tivars/models/__init__.py
 tivars/models/model.py
 tivars/models/versions.py
 tivars/tokenizer/__init__.py
-tivars/tokenizer/tokens/73.xml
-tivars/tokenizer/tokens/8X.xml
-tivars/tokenizer/tokens/scripts/__init__.py
-tivars/tokenizer/tokens/scripts/parse.py
-tivars/tokenizer/tokens/scripts/trie.py
+tivars/tokens/73.xml
+tivars/tokens/8X.xml
+tivars/tokens/scripts/__init__.py
+tivars/tokens/scripts/build.py
+tivars/tokens/scripts/formats.py
+tivars/tokens/scripts/parse.py
+tivars/tokens/scripts/tokenide.py
+tivars/tokens/scripts/trie.py
 tivars/types/__init__.py
 tivars/types/appvar.py
 tivars/types/complex.py
+tivars/types/flash.py
 tivars/types/gdb.py
 tivars/types/group.py
 tivars/types/list.py
 tivars/types/matrix.py
-tivars/types/numeric.py
 tivars/types/picture.py
 tivars/types/real.py
 tivars/types/settings.py
 tivars/types/tokenized.py
 tivars/types/json/func.default.json
 tivars/types/json/param.default.json
 tivars/types/json/polar.default.json
```

