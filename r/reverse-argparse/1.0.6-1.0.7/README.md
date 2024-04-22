# Comparing `tmp/reverse_argparse-1.0.6.tar.gz` & `tmp/reverse_argparse-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_argparse-1.0.6.tar", max compression
+gzip compressed data, was "reverse_argparse-1.0.7.tar", max compression
```

## Comparing `reverse_argparse-1.0.6.tar` & `reverse_argparse-1.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1723 2024-01-15 19:15:58.448646 reverse_argparse-1.0.6/LICENSE.md
--rw-r--r--   0        0        0     5282 2024-01-15 19:15:58.452646 reverse_argparse-1.0.6/README.md
--rw-r--r--   0        0        0     3032 2024-01-15 19:15:59.184654 reverse_argparse-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      305 2024-01-15 19:15:59.184654 reverse_argparse-1.0.6/reverse_argparse/__init__.py
--rw-r--r--   0        0        0    18717 2024-01-15 19:15:58.452646 reverse_argparse-1.0.6/reverse_argparse/reverse_argparse.py
--rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 reverse_argparse-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1711 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/LICENSE.md
+-rw-r--r--   0        0        0     5453 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/README.md
+-rw-r--r--   0        0        0     3340 2024-04-22 22:04:19.297584 reverse_argparse-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      537 2024-04-22 22:04:19.297584 reverse_argparse-1.0.7/reverse_argparse/__init__.py
+-rw-r--r--   0        0        0    19292 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/reverse_argparse/reverse_argparse.py
+-rw-r--r--   0        0        0     7123 1970-01-01 00:00:00.000000 reverse_argparse-1.0.7/PKG-INFO
```

### Comparing `reverse_argparse-1.0.6/LICENSE.md` & `reverse_argparse-1.0.7/LICENSE.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Modified BSD License
-====================
+# 3-Clause BSD License
 
-_Copyright © 2023, National Technology & Engineering Solutions of Sandia, LLC
-(NTESS).  Under the terms of Contract DE-NA0003525 with NTESS, the U.S.
-Government retains certain rights in this software.  All rights reserved._
+_Copyright © 2023–2024, National Technology & Engineering Solutions of
+Sandia, LLC (NTESS).  Under the terms of Contract DE-NA0003525 with
+NTESS, the U.S.  Government retains certain rights in this software.
+All rights reserved._
 
 Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+modification, are permitted provided that the following conditions are
+met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
 2. Redistributions in binary form must reproduce the above copyright
    notice, this list of conditions and the following disclaimer in the
    documentation and/or other materials provided with the distribution.
 3. Neither the name of Sandia National Laboratories nor the names of its
-   contributors may be used to endorse or promote products derived from this
-   software without specific prior written permission.
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS
+IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
+TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `reverse_argparse-1.0.6/README.md` & `reverse_argparse-1.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[![Code Style: black](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
+[![CodeFactor](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/badge/master)](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/overview/master)
 [![CodeQL](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql)
 [![Conda Version](https://img.shields.io/conda/v/conda-forge/reverse-argparse?label=conda-forge)](https://anaconda.org/conda-forge/reverse-argparse)
 ![Conda Downloads](https://img.shields.io/conda/d/conda-forge/reverse-argparse?label=conda-forge%20downloads)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![GitHub contributors](https://img.shields.io/github/contributors/sandialabs/reverse_argparse.svg)](https://github.com/sandialabs/reverse_argparse/graphs/contributors)
 [![Documentation Status](https://readthedocs.org/projects/reverse-argparse/badge/?version=latest)](https://reverse-argparse.readthedocs.io/en/latest/?badge=latest)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/reverse-argparse/badges/license.svg)](LICENSE.md)
-[![Linting: Pylint](https://img.shields.io/badge/Linting-Pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![License](https://anaconda.org/conda-forge/reverse-argparse/badges/license.svg)](LICENSE.md)
 [![Merged PRs](https://img.shields.io/github/issues-pr-closed-raw/sandialabs/reverse_argparse.svg?label=merged+PRs)](https://github.com/sandialabs/reverse_argparse/pulls?q=is:pr+is:merged)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7632/badge)](https://bestpractices.coreinfrastructure.org/projects/7632)
-![Anaconda-Server Badge](https://anaconda.org/conda-forge/reverse-argparse/badges/platforms.svg)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/sandialabs/reverse_argparse/badge)](https://securityscorecards.dev/viewer/?uri=github.com/sandialabs/reverse_argparse)
+![Platforms](https://anaconda.org/conda-forge/reverse-argparse/badges/platforms.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci Status](https://results.pre-commit.ci/badge/github/sandialabs/reverse_argparse/master.svg)](https://results.pre-commit.ci/latest/github/sandialabs/reverse_argparse/master)
 [![PyPI - Version](https://img.shields.io/pypi/v/reverse-argparse?label=PyPI)](https://pypi.org/project/reverse-argparse/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/reverse-argparse?label=PyPI%20downloads)
 ![Python Version](https://img.shields.io/badge/Python-3.8|3.9|3.10|3.11|3.12-blue.svg)
-[![Security: Bandit](https://img.shields.io/badge/Security-Bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 # reverse_argparse
 
 Whereas [`argparse`][argparse] is concerned with taking a bunch of command line
 arguments and parsing them, this package is intended to do the opposite; that
 is, it'll take the parsed arguments and create the effective command line
 invocation of the script that generated them.  The motivation is to be able to
@@ -91,8 +91,8 @@
 ## Credits
 
 Special thanks to [@mjsumpter][mjsumpter] for contributing to a prior iteration
 of this concept, and to [the GMS project][gms] for investing in the development
 of this package.
 
 [mjsumpter]: https://github.com/mjsumpter
-[gms]: https://github.com/SNL-GMS/GMS-PI21-OPEN/
+[gms]: https://github.com/SNL-GMS/GMS-PI25
```

### Comparing `reverse_argparse-1.0.6/pyproject.toml` & `reverse_argparse-1.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
-[pydocstyle]
-convention = "google"
-
-
 [tool.bandit.assert_used]
 skips = ["**/test_*.py"]
 
 
-[tool.black]
-line-length = 79
-
-
 [tool.commitizen]
 name = "cz_customize"
 
 
 [tool.commitizen.customize]
 schema_pattern = "(?s)(build|chore|ci|docs|feat|fix|minor|patch|perf|refactor|style|test|revert)(\\(\\S+\\))?!?:( [^\\n\\r]+)((\\n\\n.*)|(\\s*))?$"
 
 
-[tool.isort]
-profile = "black"
-line_length = 79
-
-
 [tool.poetry]
 name = "reverse_argparse"
-version = "1.0.6"
+version = "1.0.7"
 license = "LICENSE.md"
 readme = "README.md"
 keywords = ["argparse", "argument", "parse", "parsing", "command line"]
 repository = "https://github.com/sandialabs/reverse_argparse"
 description = "Generate the effective command line invocation for a script."
 documentation = "https://reverse-argparse.readthedocs.io"
 authors = [
@@ -73,14 +60,57 @@
 
 
 [tool.poetry.dev-dependencies]
 # At some point, convert from the various requirements.txt files to this
 # list of Poetry development dependencies.
 
 
+[tool.ruff]
+line-length = 79
+
+
+[tool.ruff.lint]
+extend-select = [
+    "A",
+    "B",
+    "BLE",
+    "C4",
+    "C90",
+    "D",
+    "DTZ",
+    "E",
+    "EM",
+    "ERA",
+    "EXE",
+    "FBT",
+    "NPY",
+    "PGH",
+    "PL",
+    "PT",
+    "PTH",
+    "RET",
+    "RSE",
+    "RUF",
+    "S",
+    "SIM",
+    "TID",
+    "TCH",
+    "TRY",
+    "UP",
+    "W",
+]
+ignore = [
+    "D212",
+]
+
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
+
 [tool.semantic_release]
 build_command = "python3 -m pip install poetry && poetry build"
 commit_message = """
 chore: Release v{version}
 
 Automatically generated by python-semantic-release."""
 version_variables = [
```

### Comparing `reverse_argparse-1.0.6/reverse_argparse/reverse_argparse.py` & `reverse_argparse-1.0.7/reverse_argparse/reverse_argparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-#!/usr/bin/env python3
 """
 The ``reverse_argparse`` module.
 
 Defines the :class:`ReverseArgumentParser` class for unparsing arguments
 that were already parsed via :mod:`argparse`, and the
 :func:`quote_arg_if_necessary` helper function to surround any arguments
 with spaces in them with quotes.
 """
 
+# © 2024 National Technology & Engineering Solutions of Sandia, LLC
+# (NTESS).  Under the terms of Contract DE-NA0003525 with NTESS, the
+# U.S. Government retains certain rights in this software.
+
+# SPDX-License-Identifier: BSD-3-Clause
+
 import re
 import sys
 from argparse import SUPPRESS, Action, ArgumentParser, Namespace
 from typing import List, Sequence
 
 
+BOOLEAN_OPTIONAL_ACTION_MINOR_VERSION = 9
+SHORT_OPTION_LENGTH = 2
+
+
 class ReverseArgumentParser:
     """
     Argument parsing in reverse.
 
     Whereas :class:`argparse.ArgumentParser` is concerned with taking a
     bunch of command line arguments and parsing them into a
     :class:`argparse.Namespace`, this class is intended to do the
@@ -81,15 +90,15 @@
             psr._get_optional_actions()  # pylint: disable=protected-access
             + psr._get_positional_actions()  # pylint: disable=protected-access
         )
         for action in actions:
             self._unparse_action(action)
         self._unparsed[-1] = True
 
-    def _unparse_action(self, action: Action) -> None:
+    def _unparse_action(self, action: Action) -> None:  # noqa: C901, PLR0912
         """
         Unparse a single action.
 
         Generate the command line arguments associated with the given
         ``action``, and append them to the list of arguments.
 
         Args:
@@ -125,22 +134,23 @@
             self._unparse_store_true_action(action)
         elif action_type == "_SubParsersAction":
             self._unparse_sub_parsers_action(action)
         elif action_type == "_VersionAction":  # pragma: no cover
             return
         elif (
             action_type == "BooleanOptionalAction"
-            and sys.version_info.minor >= 9
+            and sys.version_info.minor >= BOOLEAN_OPTIONAL_ACTION_MINOR_VERSION
         ):
             self._unparse_boolean_optional_action(action)
         else:  # pragma: no cover
-            raise NotImplementedError(
+            message = (
                 f"{self.__class__.__name__} does not yet support the "
                 f"unparsing of {action_type} objects."
             )
+            raise NotImplementedError(message)
 
     def _arg_is_default_and_help_is_suppressed(self, action: Action) -> bool:
         """
         See if the argument should be skipped.
 
         Determine whether the argument matches the default value and the
         corresponding help text has been suppressed.  Such cases
@@ -203,15 +213,15 @@
             A list containing only the long options (e.g., ``"--foo"``),
             and not the short ones (e.g., ``"-f"``).  Note that the list
             will be empty if there are no long options.
         """
         return [
             option
             for option in option_strings
-            if len(option) > 2
+            if len(option) > SHORT_OPTION_LENGTH
             and option[0] in self._parsers[-1].prefix_chars
             and option[1] in self._parsers[-1].prefix_chars
         ]
 
     def _get_short_option_strings(
         self, option_strings: Sequence[str]
     ) -> List[str]:
@@ -225,19 +235,20 @@
             A list containing only the short options (e.g., ``"-f"``),
             and not the short ones (e.g., ``"--foo"``).  Note that the
             list will be empty if there are no short options.
         """
         return [
             option
             for option in option_strings
-            if len(option) == 2 and option[0] in self._parsers[-1].prefix_chars
+            if len(option) == SHORT_OPTION_LENGTH
+            and option[0] in self._parsers[-1].prefix_chars
         ]
 
     def _get_option_string(
-        self, action: Action, prefer_short: bool = False
+        self, action: Action, *, prefer_short: bool = False
     ) -> str:
         """
         Get the option string for the `action`.
 
         Get the first of the long options corresponding to a given
         :class:`argparse.Action`.  If no long options are available, get
         the first of the short options.  If ``prefer_short`` is
@@ -332,18 +343,18 @@
         result = []
         if flag:
             result.append(flag)
         if not isinstance(values, list):
             values = [values]
         needs_quotes_regex = re.compile(r"(.*\s.*)")
         for value in values:
-            value = str(value)
-            if needs_quotes_regex.search(value):
-                value = needs_quotes_regex.sub(r"'\1'", value)
-            result.append(value)
+            string_value = str(value)
+            if needs_quotes_regex.search(string_value):
+                string_value = needs_quotes_regex.sub(r"'\1'", string_value)
+            result.append(string_value)
         self._append_list_of_args(result)
 
     def _unparse_store_const_action(self, action: Action) -> None:
         """
         Generate the argument for a ``store_const`` action.
 
         Args:
@@ -389,21 +400,21 @@
         if not isinstance(values, list):
             values = [values]
         result = []
         if isinstance(values[0], list):
             for entry in values:
                 tmp = [flag]
                 for value in entry:
-                    value = quote_arg_if_necessary(str(value))
-                    tmp.append(value)
+                    quoted_value = quote_arg_if_necessary(str(value))
+                    tmp.append(quoted_value)
                 result.append(tmp)
         else:
             for value in values:
-                value = quote_arg_if_necessary(str(value))
-                result.append([flag, value])
+                quoted_value = quote_arg_if_necessary(str(value))
+                result.append([flag, quoted_value])
         self._append_list_of_list_of_args(result)
 
     def _unparse_append_const_action(self, action: Action) -> None:
         """
         Generate the argument for an ``append_const`` action.
 
         Args:
@@ -419,15 +430,18 @@
 
         Args:
             action:  The :class:`_CountAction` in question.
         """
         value = getattr(self._namespace, action.dest)
         count = value if action.default is None else (value - action.default)
         flag = self._get_option_string(action, prefer_short=True)
-        if len(flag) == 2 and flag[0] in self._parsers[-1].prefix_chars:
+        if (
+            len(flag) == SHORT_OPTION_LENGTH
+            and flag[0] in self._parsers[-1].prefix_chars
+        ):
             self._append_arg(flag[0] + flag[1] * count)
         else:
             self._append_list_of_args([flag for _ in range(count)])
 
     def _unparse_sub_parsers_action(self, action: Action) -> None:
         """
         Generate the list of arguments for a subparser action.
@@ -447,18 +461,19 @@
         Raises:
             RuntimeError:  If a subparser action is somehow missing its
                 dictionary of choices.
         """
         if action.choices is None or not isinstance(
             action.choices, dict
         ):  # pragma: no cover
-            raise RuntimeError(
+            message = (
                 "This subparser action is missing its dictionary of "
                 f"choices:  {action}"
             )
+            raise RuntimeError(message)
         for subcommand, subparser in action.choices.items():
             self._parsers.append(subparser)
             self._unparsed.append(False)
             self._args.append(
                 " " * self._indent * (len(self._parsers) - 1) + subcommand
             )
             args_before = self._args.copy()
@@ -474,15 +489,15 @@
 
         Args:
             action:  The :class:`_ExtendAction` in question.
         """
         values = getattr(self._namespace, action.dest)
         if values is not None:
             self._append_list_of_args(
-                [self._get_option_string(action)] + values
+                [self._get_option_string(action), *values]
             )
 
     def _unparse_boolean_optional_action(self, action: Action) -> None:
         """
         Generate the list of arguments for a ``BooleanOptionalAction``.
 
         Args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reverse_argparse-1.0.6/PKG-INFO` & `reverse_argparse-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse_argparse
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate the effective command line invocation for a script.
 Home-page: https://github.com/sandialabs/reverse_argparse
 License: LICENSE.md
 Keywords: argparse,argument,parse,parsing,command line
 Author: Jason M. Gates
 Author-email: jmgate@sandia.gov
 Requires-Python: >=3.8
@@ -30,34 +30,34 @@
 Classifier: Typing :: Typed
 Project-URL: CI, https://github.com/sandialabs/reverse_argparse/actions
 Project-URL: Documentation, https://reverse-argparse.readthedocs.io
 Project-URL: Issues, https://github.com/sandialabs/reverse_argparse/issues
 Project-URL: Repository, https://github.com/sandialabs/reverse_argparse
 Description-Content-Type: text/markdown
 
-[![Code Style: black](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
+[![CodeFactor](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/badge/master)](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/overview/master)
 [![CodeQL](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql)
 [![Conda Version](https://img.shields.io/conda/v/conda-forge/reverse-argparse?label=conda-forge)](https://anaconda.org/conda-forge/reverse-argparse)
 ![Conda Downloads](https://img.shields.io/conda/d/conda-forge/reverse-argparse?label=conda-forge%20downloads)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![GitHub contributors](https://img.shields.io/github/contributors/sandialabs/reverse_argparse.svg)](https://github.com/sandialabs/reverse_argparse/graphs/contributors)
 [![Documentation Status](https://readthedocs.org/projects/reverse-argparse/badge/?version=latest)](https://reverse-argparse.readthedocs.io/en/latest/?badge=latest)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/reverse-argparse/badges/license.svg)](LICENSE.md)
-[![Linting: Pylint](https://img.shields.io/badge/Linting-Pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![License](https://anaconda.org/conda-forge/reverse-argparse/badges/license.svg)](LICENSE.md)
 [![Merged PRs](https://img.shields.io/github/issues-pr-closed-raw/sandialabs/reverse_argparse.svg?label=merged+PRs)](https://github.com/sandialabs/reverse_argparse/pulls?q=is:pr+is:merged)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7632/badge)](https://bestpractices.coreinfrastructure.org/projects/7632)
-![Anaconda-Server Badge](https://anaconda.org/conda-forge/reverse-argparse/badges/platforms.svg)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/sandialabs/reverse_argparse/badge)](https://securityscorecards.dev/viewer/?uri=github.com/sandialabs/reverse_argparse)
+![Platforms](https://anaconda.org/conda-forge/reverse-argparse/badges/platforms.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci Status](https://results.pre-commit.ci/badge/github/sandialabs/reverse_argparse/master.svg)](https://results.pre-commit.ci/latest/github/sandialabs/reverse_argparse/master)
 [![PyPI - Version](https://img.shields.io/pypi/v/reverse-argparse?label=PyPI)](https://pypi.org/project/reverse-argparse/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/reverse-argparse?label=PyPI%20downloads)
 ![Python Version](https://img.shields.io/badge/Python-3.8|3.9|3.10|3.11|3.12-blue.svg)
-[![Security: Bandit](https://img.shields.io/badge/Security-Bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 # reverse_argparse
 
 Whereas [`argparse`][argparse] is concerned with taking a bunch of command line
 arguments and parsing them, this package is intended to do the opposite; that
 is, it'll take the parsed arguments and create the effective command line
 invocation of the script that generated them.  The motivation is to be able to
@@ -127,9 +127,9 @@
 ## Credits
 
 Special thanks to [@mjsumpter][mjsumpter] for contributing to a prior iteration
 of this concept, and to [the GMS project][gms] for investing in the development
 of this package.
 
 [mjsumpter]: https://github.com/mjsumpter
-[gms]: https://github.com/SNL-GMS/GMS-PI21-OPEN/
+[gms]: https://github.com/SNL-GMS/GMS-PI25
```

