# Comparing `tmp/formaldict-1.0.5.tar.gz` & `tmp/formaldict-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formaldict-1.0.5.tar", max compression
+gzip compressed data, was "formaldict-1.0.6.tar", max compression
```

## Comparing `formaldict-1.0.5.tar` & `formaldict-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1456 2022-08-20 21:21:41.631502 formaldict-1.0.5/LICENSE
--rw-r--r--   0        0        0     1292 2022-08-20 21:21:41.631502 formaldict-1.0.5/README.rst
--rw-r--r--   0        0        0      213 2022-08-20 21:21:41.639502 formaldict-1.0.5/formaldict/__init__.py
--rw-r--r--   0        0        0    19946 2022-08-20 21:21:41.639502 formaldict-1.0.5/formaldict/core.py
--rw-r--r--   0        0        0      245 2022-08-20 21:21:41.639502 formaldict-1.0.5/formaldict/exceptions.py
--rw-r--r--   0        0        0      148 2022-08-20 21:21:41.639502 formaldict-1.0.5/formaldict/version.py
--rw-r--r--   0        0        0     1852 2022-08-20 21:21:58.699696 formaldict-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2176 2022-08-20 21:22:03.430120 formaldict-1.0.5/setup.py
--rw-r--r--   0        0        0     2383 2022-08-20 21:22:03.430446 formaldict-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-23 20:20:11.312636 formaldict-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1248 2024-04-23 20:20:11.312636 formaldict-1.0.6/README.md
+-rw-r--r--   0        0        0      159 2024-04-23 20:20:11.320636 formaldict-1.0.6/formaldict/__init__.py
+-rw-r--r--   0        0        0    19981 2024-04-23 20:20:11.320636 formaldict-1.0.6/formaldict/core.py
+-rw-r--r--   0        0        0      245 2024-04-23 20:20:11.320636 formaldict-1.0.6/formaldict/exceptions.py
+-rw-r--r--   0        0        0       77 2024-04-23 20:20:11.320636 formaldict-1.0.6/formaldict/version.py
+-rw-r--r--   0        0        0     2109 2024-04-23 20:20:31.080949 formaldict-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 formaldict-1.0.6/PKG-INFO
```

### Comparing `formaldict-1.0.5/LICENSE` & `formaldict-1.0.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `formaldict-1.0.5/README.rst` & `formaldict-1.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,31 @@
-formaldict
-###########
+# formaldict
 
-``formaldict`` provides the constructs for parsing structured dictionaries
-that adhere to a schema. Along with a simple and flexible schema definition
-to parse and validate dictionaries, ``formaldict`` is integrated with
-`python-prompt-toolkit <https://github.com/prompt-toolkit/python-prompt-toolkit>`__.
-This integration allows users to easily construct flows for command line
-interfaces (CLIs) when parsing structured user input.
+`formaldict` provides the constructs for parsing structured dictionaries that adhere to a schema. Along with a simple and flexible schema definition to parse and validate dictionaries, `formaldict` is integrated with [python-prompt-toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit). This integration allows users to easily construct flows for command line interfaces (CLIs) when parsing structured user input.
 
-Below is an example user input flow constructed with a ``formaldict``
-schema used by `git-tidy <https://github.com/jyveapp/git-tidy>`__:
+Below is an example user input flow constructed with a `formaldict` schema used by [git-tidy](https://github.com/Opus10/git-tidy):
 
-.. image:: https://raw.githubusercontent.com/jyveapp/formaldict/master/docs/_static/prompt.gif
-   :width: 600
+![Usage](https://raw.githubusercontent.com/Opus10/formaldict/main/docs/static/prompt.gif)
 
-Check out the `docs <https://formaldict.readthedocs.io/>`__ for a
-tutorial on how to use ``formaldict`` as the backbone for parsing
-structured input in your library.
+Check out the [docs](https://formaldict.readthedocs.io/) for a tutorial on how to use `formaldict` as the backbone for parsing structured input in your library.
 
-Documentation
-=============
+## Documentation
 
-`View the formaldict docs here
-<https://formaldict.readthedocs.io/>`_.
+[View the formaldict docs here](https://formaldict.readthedocs.io/).
 
-Installation
-============
+## Installation
 
-Install formaldict with::
+Install formaldict with:
 
     pip3 install formaldict
 
+## Contributing Guide
 
-Contributing Guide
-==================
+For information on setting up formaldict for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-For information on setting up formaldict for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+## Compatibility
 
+`formaldict` is compatible with Python 3.8 - 3.12.
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
```

### Comparing `formaldict-1.0.5/formaldict/core.py` & `formaldict-1.0.6/formaldict/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 This module contains the `Schema`, the parsed
 `FormalDict`, and the `Errors` from any parsing/validation failures
 
 .. note::
 
     The ``formaldict`` module will eventually be its own library.
 """
+
 import collections.abc
 import copy
 import datetime as dt
 import re
 
 import dateutil.parser
 import kmatch
 import prompt_toolkit
+import prompt_toolkit.validation
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.formatted_text import HTML
-import prompt_toolkit.validation
 
 from . import exceptions
 
 
 class _ValueValidator(prompt_toolkit.validation.Validator):
     """
     Custom validator class for prompt_toolkit. Performs validation
     on input in the same way schemas are validated
     """
 
-    def __init__(self, *args, schema=None, label=None, **kwargs):
+    def __init__(self, *args, schema, label, **kwargs):
         self._schema = schema
         self._label = label
         super().__init__(*args, **kwargs)
 
     def validate(self, document):
         text = document.text
         try:
             self._schema._parse_entry(self._label, text)
         except exceptions.ValidationError as exc:
             raise prompt_toolkit.validation.ValidationError(
                 message=str(exc), cursor_position=len(text)
-            )
+            ) from exc
 
 
 class Errors(collections.abc.Mapping):
     """
     Collects errors found when validating a `Schema`
     """
 
@@ -460,33 +461,34 @@
         if entry_schema["condition"] is None:
             return True
         elif isinstance(entry_schema["condition"], bool):
             return entry_schema["condition"]
         else:
             return entry_schema["condition"].match(data)
 
-    def parse(self, data, strict=False):
+    def parse(self, data, strict=False) -> FormalDict:
         """
         Parse data based on the schema.
 
         Args:
             strict (boolean, default=False): If True, add a
                 ValidationError to self.errors if any keys in the entry
                 are not present in the schema.
 
         Returns:
-            dict: The parsed data
+            The parsed data
 
         Todo:
             Allow passing in default values to override any defaults in the
             schema.
         """
         parsed = {}
         errors = Errors()
         condition_failed_labels = set()
+        label = ""
         for entry_schema in self:
             try:
                 label = entry_schema["label"]
                 if not self.passes_condition(entry_schema, parsed):
                     condition_failed_labels.add(label)
                     continue
 
@@ -536,24 +538,24 @@
         entry_schema = self[label]
         prompt_text = f'{entry_schema["name"]}: '
         if entry_schema["multiline"]:
             prompt_text += "\n> "
 
         return prompt_text
 
-    def prompt(self, defaults=None):
+    def prompt(self, defaults=None) -> FormalDict:
         """
         Prompt for input of all entries in the schema
 
         Args:
             defaults (dict, default=None): Default values for the schema
                 that should be used in place of any other declared defaults
 
         Returns:
-            dict: The parsed information, which also validates against the
+            The parsed information, which also validates against the
             `Schema`.
         """
         defaults = defaults or {}
         data = {}
 
         for entry_schema in self:
             if not self.passes_condition(entry_schema, data):
```

### Comparing `formaldict-1.0.5/pyproject.toml` & `formaldict-1.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,94 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py37']
-
 [tool.coverage.run]
 branch = true
 source = ["formaldict"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "formaldict"
 packages = [
   { include = "formaldict" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.0.5"
+version = "1.0.6"
 description = "Formal structured dictionaries parsed from a schema"
 authors = ["Wes Kendall"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 license = "BSD-3-Clause"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/Opus10/formaldict"
 repository = "https://github.com/Opus10/formaldict"
 documentation = "https://formaldict.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
-importlib_metadata = { version = ">=4", python = "~3.7" }
+python = ">=3.8.0,<4"
 kmatch = ">=0.3.0"
 python-dateutil = ">=2.8.1"
 prompt-toolkit = ">=3.0.2"
 
 [tool.poetry.dev-dependencies]
-black = "22.1.0"
-flake8 = "3.9.2"
-flake8-bugbear = "22.1.11"
-flake8-comprehensions = "3.8.0"
-flake8-import-order = "0.18.1"
-flake8-logging-format = "0.6.0"
-flake8-mutable = "1.2.0"
-footing = "*"
-git-tidy = "1.1.1"
+git-tidy = "1.2.0"
+pytest = "7.4.2"
+pytest-cov = "4.1.0"
+pytest-dotenv = "0.5.2"
 pytest-mock = "3.7.0"
-myst-parser = "0.18.0"
-pytest = "6.2.5"
-pytest-cov = "3.0.0"
-Sphinx = "4.4.0"
-sphinx-rtd-theme = "1.0.0"
-tox = "3.24.5"
+tox = "4.11.3"
+ruff = "0.3.7"
+pyright = "1.1.358"
+mkdocs = "1.5.3"
+black = "24.4.0"
+mkdocs-material = "9.5.18"
+mkdocstrings-python = "1.9.2"
+footing = "*"
+setuptools = "*"
+poetry-core = "*"
+typing-extensions = "4.11.0"
+pyyaml = "5.3.1"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "formaldict/tests"
 norecursedirs = ".venv"
+
+[tool.ruff]
+lint.select = ["E", "F", "B", "I", "G", "C4"]
+line-length = 99
+target-version = "py38"
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/migrations/**",
+    "**/tests/**",
+]
+pythonVersion = "3.8"
+typeCheckingMode = "standard"
```

### Comparing `formaldict-1.0.5/PKG-INFO` & `formaldict-1.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,58 @@
 Metadata-Version: 2.1
 Name: formaldict
-Version: 1.0.5
+Version: 1.0.6
 Summary: Formal structured dictionaries parsed from a schema
 Home-page: https://github.com/Opus10/formaldict
 License: BSD-3-Clause
 Author: Wes Kendall
-Requires-Python: >=3.7.0,<4
+Requires-Python: >=3.8.0,<4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: kmatch (>=0.3.0)
 Requires-Dist: prompt-toolkit (>=3.0.2)
 Requires-Dist: python-dateutil (>=2.8.1)
 Project-URL: Documentation, https://formaldict.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/formaldict
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-formaldict
-###########
+# formaldict
 
-``formaldict`` provides the constructs for parsing structured dictionaries
-that adhere to a schema. Along with a simple and flexible schema definition
-to parse and validate dictionaries, ``formaldict`` is integrated with
-`python-prompt-toolkit <https://github.com/prompt-toolkit/python-prompt-toolkit>`__.
-This integration allows users to easily construct flows for command line
-interfaces (CLIs) when parsing structured user input.
+`formaldict` provides the constructs for parsing structured dictionaries that adhere to a schema. Along with a simple and flexible schema definition to parse and validate dictionaries, `formaldict` is integrated with [python-prompt-toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit). This integration allows users to easily construct flows for command line interfaces (CLIs) when parsing structured user input.
 
-Below is an example user input flow constructed with a ``formaldict``
-schema used by `git-tidy <https://github.com/jyveapp/git-tidy>`__:
+Below is an example user input flow constructed with a `formaldict` schema used by [git-tidy](https://github.com/Opus10/git-tidy):
 
-.. image:: https://raw.githubusercontent.com/jyveapp/formaldict/master/docs/_static/prompt.gif
-   :width: 600
+![Usage](https://raw.githubusercontent.com/Opus10/formaldict/main/docs/static/prompt.gif)
 
-Check out the `docs <https://formaldict.readthedocs.io/>`__ for a
-tutorial on how to use ``formaldict`` as the backbone for parsing
-structured input in your library.
+Check out the [docs](https://formaldict.readthedocs.io/) for a tutorial on how to use `formaldict` as the backbone for parsing structured input in your library.
 
-Documentation
-=============
+## Documentation
 
-`View the formaldict docs here
-<https://formaldict.readthedocs.io/>`_.
+[View the formaldict docs here](https://formaldict.readthedocs.io/).
 
-Installation
-============
+## Installation
 
-Install formaldict with::
+Install formaldict with:
 
     pip3 install formaldict
 
+## Contributing Guide
 
-Contributing Guide
-==================
+For information on setting up formaldict for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-For information on setting up formaldict for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+## Compatibility
 
+`formaldict` is compatible with Python 3.8 - 3.12.
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
```

