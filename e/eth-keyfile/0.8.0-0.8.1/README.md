# Comparing `tmp/eth-keyfile-0.8.0.tar.gz` & `tmp/eth_keyfile-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-keyfile-0.8.0.tar", last modified: Wed Feb 28 20:13:15 2024, max compression
+gzip compressed data, was "eth_keyfile-0.8.1.tar", last modified: Tue Apr 23 20:28:47 2024, max compression
```

## Comparing `eth-keyfile-0.8.0.tar` & `eth_keyfile-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8426 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6838 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/eth_keyfile/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      236 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/eth_keyfile/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9411 2024-02-28 18:51:08.000000 eth-keyfile-0.8.0/eth_keyfile/keyfile.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/eth_keyfile/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/eth_keyfile.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8426 2024-02-28 20:13:14.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      496 2024-02-28 20:13:15.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-02-28 20:13:14.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-11-02 19:18:05.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      260 2024-02-28 20:13:14.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       12 2024-02-28 20:13:14.000000 eth-keyfile-0.8.0/eth_keyfile.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3460 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1997 2024-02-28 20:13:01.000000 eth-keyfile-0.8.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/tests/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4440 2024-02-28 18:51:08.000000 eth-keyfile-0.8.0/tests/conftest.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-02-28 20:13:15.046083 eth-keyfile-0.8.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       56 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/tests/core/test_import.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1478 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/tests/test_keyfile_creation.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      433 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/tests/test_keyfile_loading.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1462 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/tests/test_loading_from_file.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      840 2024-02-28 17:21:48.000000 eth-keyfile-0.8.0/tests/test_readme_examples.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 20:28:47.620029 eth_keyfile-0.8.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-11-27 12:53:38.000000 eth_keyfile-0.8.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      196 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8475 2024-04-23 20:28:47.620029 eth_keyfile-0.8.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6836 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 20:28:47.616029 eth_keyfile-0.8.1/eth_keyfile/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      236 2023-11-27 12:53:38.000000 eth_keyfile-0.8.1/eth_keyfile/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     9411 2024-04-04 23:34:53.000000 eth_keyfile-0.8.1/eth_keyfile/keyfile.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-11-27 12:53:38.000000 eth_keyfile-0.8.1/eth_keyfile/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 20:28:47.616029 eth_keyfile-0.8.1/eth_keyfile.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     8475 2024-04-23 20:28:47.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      533 2024-04-23 20:28:47.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-23 20:28:47.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-11-03 08:53:27.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      260 2024-04-23 20:28:47.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       12 2024-04-23 20:28:47.000000 eth_keyfile-0.8.1/eth_keyfile.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3456 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-23 20:28:47.620029 eth_keyfile-0.8.1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2047 2024-04-23 20:28:41.000000 eth_keyfile-0.8.1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 20:28:47.616029 eth_keyfile-0.8.1/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 20:28:47.616029 eth_keyfile-0.8.1/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4437 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/conftest.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      107 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/test_import_and_version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1478 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/test_keyfile_creation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      433 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/test_keyfile_loading.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1462 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/test_loading_from_file.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      835 2024-04-19 21:41:24.000000 eth_keyfile-0.8.1/tests/core/test_readme_examples.py
```

### Comparing `eth-keyfile-0.8.0/LICENSE` & `eth_keyfile-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-keyfile-0.8.0/PKG-INFO` & `eth_keyfile-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-keyfile
-Version: 0.8.0
+Version: 0.8.1
 Summary: eth-keyfile: A library for handling the encrypted keyfiles used to store ethereum private keys
 Home-page: https://github.com/ethereum/eth-keyfile
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Requires-Dist: eth-keys>=0.4.0
 Requires-Dist: pycryptodome<4,>=3.6.6
 Provides-Extra: dev
@@ -45,15 +46,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-keyfile.svg)](https://badge.fury.io/py/eth-keyfile)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-keyfile.svg)](https://pypi.python.org/pypi/eth-keyfile)
 
 A library for handling the encrypted keyfiles used to store ethereum private keys
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-keyfile.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-keyfile`.  The PyPi package was also renamed from `ethereum-keyfile` to `eth-keyfile`.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/main/CHANGELOG.rst).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-keyfile
 ```
```

### Comparing `eth-keyfile-0.8.0/README.md` & `eth_keyfile-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-keyfile.svg)](https://badge.fury.io/py/eth-keyfile)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-keyfile.svg)](https://pypi.python.org/pypi/eth-keyfile)
 
 A library for handling the encrypted keyfiles used to store ethereum private keys
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-keyfile.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-keyfile`.  The PyPi package was also renamed from `ethereum-keyfile` to `eth-keyfile`.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/main/CHANGELOG.rst).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-keyfile
 ```
```

### Comparing `eth-keyfile-0.8.0/eth_keyfile/keyfile.py` & `eth_keyfile-0.8.1/eth_keyfile/keyfile.py`

 * *Files identical despite different names*

### Comparing `eth-keyfile-0.8.0/eth_keyfile.egg-info/PKG-INFO` & `eth_keyfile-0.8.1/eth_keyfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-keyfile
-Version: 0.8.0
+Version: 0.8.1
 Summary: eth-keyfile: A library for handling the encrypted keyfiles used to store ethereum private keys
 Home-page: https://github.com/ethereum/eth-keyfile
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Requires-Dist: eth-keys>=0.4.0
 Requires-Dist: pycryptodome<4,>=3.6.6
 Provides-Extra: dev
@@ -45,15 +46,15 @@
 [![PyPI version](https://badge.fury.io/py/eth-keyfile.svg)](https://badge.fury.io/py/eth-keyfile)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-keyfile.svg)](https://pypi.python.org/pypi/eth-keyfile)
 
 A library for handling the encrypted keyfiles used to store ethereum private keys
 
 > This library and repository was previously located at https://github.com/pipermerriam/ethereum-keyfile.  It was transferred to the Ethereum foundation github in November 2017 and renamed to `eth-keyfile`.  The PyPi package was also renamed from `ethereum-keyfile` to `eth-keyfile`.
 
-Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/master/CHANGELOG.rst).
+Read more in the documentation below. [View the change log](https://github.com/ethereum/eth-keyfile/blob/main/CHANGELOG.rst).
 
 ## Quickstart
 
 ```sh
 python -m pip install eth-keyfile
 ```
```

### Comparing `eth-keyfile-0.8.0/pyproject.toml` & `eth_keyfile-0.8.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.autoflake]
-remove_all_unused_imports = "True"
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
-combine_as_imports = "True"
+combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
-force_sort_within_sections = "True"
-known_third_party = "hypothesis,pytest"
+force_sort_within_sections = true
+honor_noqa = true
 known_first_party = "eth_keyfile"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
-check_untyped_defs = "True"
-disallow_incomplete_defs = "True"
-disallow_untyped_defs = "True"
-disallow_any_generics = "True"
-disallow_untyped_calls = "True"
-disallow_untyped_decorators = "True"
-disallow_subclassing_any = "True"
-ignore_missing_imports = "True"
-strict_optional = "True"
-strict_equality = "True"
-warn_redundant_casts = "True"
-warn_return_any = "True"
-warn_unused_configs = "True"
-warn_unused_ignores = "True"
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
+ignore_missing_imports = true
+strict_equality = true
+strict_optional = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_configs = true
+warn_unused_ignores = true
 
 
 [tool.pydocstyle]
 # All error codes found here:
 # http://www.pydocstyle.org/en/3.0.0/error_codes.html
 #
 # Ignored:
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = "True"
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
-# Read https://github.com/ethereum/eth-keyfile/blob/master/newsfragments/README.md for instructions
-package = "eth_keyfile"
-filename = "CHANGELOG.rst"
+# Read https://github.com/ethereum/eth-keyfile/blob/main/newsfragments/README.md for instructions
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "eth-keyfile v{version} ({project_date})"
+filename = "CHANGELOG.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-keyfile/issues/{issue}>`__"
+package = "eth_keyfile"
+title_format = "eth-keyfile v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `eth-keyfile-0.8.0/setup.py` & `eth_keyfile-0.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import (
     find_packages,
     setup,
 )
 
 extras_require = {
     "dev": [
@@ -32,15 +31,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-keyfile",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="0.8.0",
+    version="0.8.1",
     description=(
         "eth-keyfile: A library for handling the encrypted keyfiles used to store "
         "ethereum private keys"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
@@ -54,21 +53,22 @@
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
     py_modules=["eth_keyfile"],
     license="MIT",
     zip_safe=False,
     keywords="ethereum",
-    packages=find_packages(exclude=["tests", "tests.*"]),
+    packages=find_packages(exclude=["scripts", "scripts.*", "tests", "tests.*"]),
     package_data={"eth_keyfile": ["py.typed"]},
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `eth-keyfile-0.8.0/tests/conftest.py` & `eth_keyfile-0.8.1/tests/core/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 import os
-
 import pytest
 
 import eth_keyfile
 
 FIXTURES_FILE_PATH = os.path.join(
-    os.path.dirname(os.path.dirname((eth_keyfile.__file__))),
+    os.path.dirname(os.path.dirname(eth_keyfile.__file__)),
     "fixtures",
     "KeyStoreTests",
     "basic_tests.json",
 )
 
 MEW_KEYFILE = {
     "json": {
```

### Comparing `eth-keyfile-0.8.0/tests/test_keyfile_creation.py` & `eth_keyfile-0.8.1/tests/core/test_keyfile_creation.py`

 * *Files identical despite different names*

### Comparing `eth-keyfile-0.8.0/tests/test_loading_from_file.py` & `eth_keyfile-0.8.1/tests/core/test_loading_from_file.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
+import pytest
 
 from eth_utils import (
     decode_hex,
 )
-import pytest
 
 from eth_keyfile.keyfile import (
     create_keyfile_json,
     extract_key_from_keyfile,
     load_keyfile,
 )
```

### Comparing `eth-keyfile-0.8.0/tests/test_readme_examples.py` & `eth_keyfile-0.8.1/tests/core/test_readme_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Run doctests in the given block of code."""
     parser = doctest.DocTestParser()
     test = parser.get_doctest(code, {}, "extracted_doctests", "extracted", 0)
     runner = doctest.DocTestRunner()
     runner.run(test)
 
 
-with open("README.md", "r") as f:
+with open("README.md") as f:
     markdown_content = f.read()
 
 code_to_test = extract_doctests(markdown_content)
 run_doctests(code_to_test)
 
 
 def test_readme_examples():
```

