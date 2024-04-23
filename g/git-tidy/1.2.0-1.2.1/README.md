# Comparing `tmp/git-tidy-1.2.0.tar.gz` & `tmp/git_tidy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-tidy-1.2.0.tar", max compression
+gzip compressed data, was "git_tidy-1.2.1.tar", max compression
```

## Comparing `git-tidy-1.2.0.tar` & `git_tidy-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1456 2023-03-26 15:24:21.265852 git-tidy-1.2.0/LICENSE
--rw-r--r--   0        0        0     1989 2023-03-26 15:24:21.265852 git-tidy-1.2.0/README.rst
--rw-r--r--   0        0        0     2131 2023-03-26 15:24:37.653896 git-tidy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/__init__.py
--rw-r--r--   0        0        0     4055 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/cli.py
--rw-r--r--   0        0        0    27175 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/core.py
--rw-r--r--   0        0        0      759 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/exceptions.py
--rw-r--r--   0        0        0     4605 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/github.py
--rw-r--r--   0        0        0      960 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/utils.py
--rw-r--r--   0        0        0      146 2023-03-26 15:24:21.273851 git-tidy-1.2.0/tidy/version.py
--rw-r--r--   0        0        0     3268 2023-03-26 15:24:41.903396 git-tidy-1.2.0/setup.py
--rw-r--r--   0        0        0     3187 2023-03-26 15:24:41.903929 git-tidy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-23 21:18:27.761603 git_tidy-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1578 2024-04-23 21:18:27.761603 git_tidy-1.2.1/README.md
+-rw-r--r--   0        0        0     2382 2024-04-23 21:18:52.141938 git_tidy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      354 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/__init__.py
+-rw-r--r--   0        0        0     4056 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/cli.py
+-rw-r--r--   0        0        0    27245 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/core.py
+-rw-r--r--   0        0        0      759 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/exceptions.py
+-rw-r--r--   0        0        0     4588 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/github.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:18:27.769603 git_tidy-1.2.1/tidy/py.typed
+-rw-r--r--   0        0        0      960 2024-04-23 21:18:27.773603 git_tidy-1.2.1/tidy/utils.py
+-rw-r--r--   0        0        0       75 2024-04-23 21:18:27.773603 git_tidy-1.2.1/tidy/version.py
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 git_tidy-1.2.1/PKG-INFO
```

### Comparing `git-tidy-1.2.0/LICENSE` & `git_tidy-1.2.1/LICENSE`

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

### Comparing `git-tidy-1.2.0/README.rst` & `git_tidy-1.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,38 @@
-git-tidy
-########
+# git-tidy
 
-``git-tidy`` is a set of git extensions for:
+`git-tidy` is a set of git extensions for:
 
-1. Keeping your git logs tidy with ease. ``git tidy-commit`` guides
-   users through a structured commit with a configurable schema.
-   ``git tidy-squash`` squashes messy commits into one tidy commit.
-2. Linting a commit log. ``git tidy-lint`` verifies that commits
-   match the schema. If a user uses ``git tidy-commit``, commits
-   will *always* validate.
-3. Rendering a commit log. ``git tidy-log`` can render commits from
-   any range and can render structured commits from a configurable
-   `Jinja <https://jinja.palletsprojects.com/en/2.11.x/>`__ template.
-   Want to automatically generate release notes? ``git tidy-log`` can
-   be configured to group and render commits based on the schema.
-
-.. image:: https://raw.githubusercontent.com/jyveapp/git-tidy/master/docs/_static/tidy-commit.gif
-    :width: 600
-
-Documentation
-=============
-
-`View the git-tidy docs here
-<https://git-tidy.readthedocs.io/>`_ for a complete tutorial on using
-``git-tidy``.
-
-Installation
-============
+1. Keeping your git logs tidy with ease. `git tidy-commit` guides users through a structured commit with a configurable schema. `git tidy-squash` squashes messy commits into one tidy commit.
+2. Linting a commit log. `git tidy-lint` verifies that commits match the schema. If a user uses `git tidy-commit`, commits will *always* validate.
+3. Rendering a commit log. `git tidy-log` can render commits from any range and can render structured commits from a configurable [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) template. Want to automatically generate release notes? `git tidy-log` can be configured to group and render commits based on the schema.
 
-``git-tidy`` can be installed a number of ways. The preferred way
-on OSX is with `homebrew <brew.sh>`__ ::
+![Example](https://raw.githubusercontent.com/jyveapp/git-tidy/main/docs/static/tidy-commit.gif)
 
-    brew tap jyveapp/homebrew-tap
-    brew install git-tidy
+## Documentation
 
-If not on OSX, one can install ``git-tidy`` system-wide with
-`pipx <https://github.com/pipxproject/pipx>`__::
+[View the git-tidy docs here](https://git-tidy.readthedocs.io/) for a complete tutorial on using `git-tidy`.
+
+## Installation
+
+One can install `git-tidy` system-wide with [pipx](https://github.com/pipxproject/pipx):
 
     pipx install git-tidy
 
-``git-tidy`` can also be installed with pip. Be sure to install it system-wide
-so that ``git-tidy``'s execution is not tied to a virtual environment::
+or pip:
 
     pip3 install git-tidy
 
+**Note** `git-tidy` depends on git at a version of 2.22 or higher. OSX users can upgrade to the latest `git` version with [homebrew](brew.sh) using `brew install git`.
 
-.. note::
-
-  ``git-tidy`` depends on git at a version of 2.22 or higher. OSX
-  users can upgrade to the latest ``git`` version with
-  `homebrew <brew.sh>`__ using ``brew install git``.
+## Compatibility
 
+`git-tidy` is compatible with Python 3.8 - 3.12.
 
-Contributing Guide
-==================
+## Contributing Guide
 
-For information on setting up git-tidy for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+For information on setting up git-tidy for development and contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
 - @tomage (Tómas Árni Jónasson)
```

### Comparing `git-tidy-1.2.0/pyproject.toml` & `git_tidy-1.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,105 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py37']
-
 [tool.coverage.run]
 branch = true
 source = ["tidy"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
+    "if TYPE_CHECKING:",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "git-tidy"
 packages = [
   { include = "tidy" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.2.0"
+version = "1.2.1"
 description = "Tidy git commit messages, linting, and logging"
 authors = ["Wes Kendall", "Tómas Árni Jónasson"]
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
 homepage = "https://github.com/Opus10/git-tidy"
 repository = "https://github.com/Opus10/git-tidy"
 documentation = "https://git-tidy.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
-importlib_metadata = { version = ">=4", python = "~3.7" }
+python = ">=3.8.0,<4"
 click = ">7.0"
 formaldict = ">0.2.0"
 jinja2 = ">2.10.3"
 packaging = ">20.0"
 python-dateutil = ">2.8.1"
-pyyaml = ">5.1.2"
+pyyaml = ">=5.1.2,<=5.3.1"
 requests = ">2.22.0"
 
 [tool.poetry.dev-dependencies]
-black = "22.3.0"
-flake8 = "3.9.2"
-flake8-bugbear = "22.1.11"
-flake8-comprehensions = "3.8.0"
-flake8-import-order = "0.18.1"
-flake8-logging-format = "0.6.0"
-flake8-mutable = "1.2.0"
-footing = "*"
-myst-parser = "0.18.0"
-pytest = "6.2.5"
-pytest-cov = "3.0.0"
-pytest-mock = "3.7.0"
+pytest = "7.4.2"
+pytest-cov = "4.1.0"
+pytest-dotenv = "0.5.2"
+pytest-mock = "3.14.0"
 pytest-responses = "0.5.0"
-Sphinx = "4.4.0"
-sphinx-click = "3.0.0"
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
 
 [tool.poetry.scripts]
 git-tidy = 'tidy.cli:tidy'
 git-tidy-commit = 'tidy.cli:commit'
 git-tidy-lint = 'tidy.cli:lint'
 git-tidy-log = 'tidy.cli:log'
 git-tidy-squash = 'tidy.cli:squash'
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "tidy/tests"
 norecursedirs = ".venv"
 
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

### Comparing `git-tidy-1.2.0/tidy/cli.py` & `git_tidy-1.2.1/tidy/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 * ``git-tidy`` - Prints version information
 * ``git-tidy-commit`` - Performs a tidy commit
 * ``git-tidy-log`` - Renders templated commit messages
 * ``git-tidy-lint`` - Validates structure of commit messages
 * ``git-tidy-squash`` - Squashes commit messages into a single tidy commit
 """
+
 import sys
 
 import click
 import pkg_resources
 
 from tidy import core
```

### Comparing `git-tidy-1.2.0/tidy/core.py` & `git_tidy-1.2.1/tidy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 The core git tidy API
 """
 
+from __future__ import annotations
+
 import collections.abc
 import io
 import os
 import re
 import subprocess
 import tempfile
+from typing import TYPE_CHECKING
 
 import dateutil.parser
 import formaldict
 import jinja2
-from packaging import version
 import yaml
+from packaging import version
 
-from tidy import exceptions
-from tidy import github
-from tidy import utils
+from tidy import exceptions, github, utils
 
+if TYPE_CHECKING:
+    from datetime import datetime
 
 # The default tidy log Jinja template
 DEFAULT_LOG_TEMPLATE = """
 {% for tag, commits_by_tag in commits.group('tag').items() %}
 ## {{ tag|default('Unreleased', True) }} {% if tag.date %}({{ tag.date.date() }}){% endif %}
 {% for commit in commits_by_tag %}
 - {{ commit.summary }} [{{ commit.author_name }}, {{ commit.sha[:7] }}]
@@ -196,35 +199,35 @@
 class Tag(collections.UserString):
     """A git tag."""
 
     def __init__(self, tag):
         self.data = tag
 
     @classmethod
-    def from_sha(cls, sha, tag_match=None):
+    def from_sha(cls, sha, tag_match=None) -> Tag:
         """
         Create a Tag object from a sha or return None if there is no
         associated tag
 
         Returns:
-            Tag: A constructed tag or ``None`` if no tags contain the commit.
+            A constructed tag or ``None`` if no tags contain the commit.
         """
         describe_cmd = f"git describe {sha} --contains"
         if tag_match:
             describe_cmd += f" --match={tag_match}"
 
         rev = (
             utils.shell_stdout(describe_cmd, check=False, stderr=subprocess.PIPE)
             .replace("~", ":")
             .replace("^", ":")
         )
         return cls(rev.split(":")[0]) if rev else None
 
     @property
-    def date(self):
+    def date(self) -> datetime:
         """
         Parse the date of the tag
 
         Returns:
             datetime: The tag parsed as a datetime object.
         """
         if not hasattr(self, "_date"):
@@ -370,68 +373,67 @@
 
     def __getitem__(self, i):
         return self._commits[i]
 
     def __len__(self):
         return len(self._commits)
 
-    def filter(self, attr, value, match=False):
+    def filter(self, attr, value, match=False) -> Commits:
         """Filter commits by an attribute
 
         Args:
             attr (str): The name of the attribute on the `Commit` object.
             value (str|bool): The value to filter by.
             match (bool, default=False): Treat ``value`` as a regex pattern and
                 match against it.
 
         Returns:
-            `Commits`: The filtered commits.
+            The filtered commits.
         """
         return Commits(
             [commit for commit in self if _equals(getattr(commit, attr), value, match=match)]
         )
 
-    def exclude(self, attr, value, match=False):
+    def exclude(self, attr, value, match=False) -> Commits:
         """Exclude commits by an attribute
 
         Args:
             attr (str): The name of the attribute on the `Commit` object.
             value (str|bool): The value to exclude by.
             match (bool, default=False): Treat ``value`` as a regex pattern and
                 match against it.
 
         Returns:
-            `Commits`: The excluded commits.
+            The excluded commits.
         """
         return Commits(
             [commit for commit in self if not _equals(getattr(commit, attr), value, match=match)]
         )
 
     def group(
         self,
         attr,
         ascending_keys=False,
         descending_keys=False,
         none_key_first=False,
         none_key_last=False,
-    ):
+    ) -> dict[str, Commits]:
         """Group commits by an attribute
 
         Args:
             attr (str): The attribute to group by.
             ascending_keys (bool, default=False): Sort the keys in ascending
                 order.
             descending_keys (bool, default=False): Sort the keys in descending
                 order.
             none_key_first (bool, default=False): Make the "None" key be first.
             none_key_last (bool, default=False): Make the "None" key be last.
 
         Returns:
-            `collections.OrderedDict`: A dictionary of `Commits` keyed on
-            groups.
+            A dictionary of `Commits` keyed on groups.
         """
         if any([ascending_keys, descending_keys]) and not any([none_key_first, none_key_last]):
             # If keys are sorted, default to making the "None" key last
             none_key_last = True
 
         # Get the natural ordering of the keys
         keys = list(
@@ -588,29 +590,28 @@
     rendered = template.render(schema=schema)
 
     _output(path=output, value=rendered)
 
     return rendered
 
 
-def commit(no_verify=False, allow_empty=False, defaults=None):
+def commit(no_verify=False, allow_empty=False, defaults=None) -> subprocess.CompletedProcess:
     """
     Performs a tidy git commit.
 
     Args:
         no_verify (bool, default=False): True if ignoring
             pre-commit hooks
         allow_empty (bool, default=False): True if an empty
             commit should be allowed
         defaults (dict, default=None): Defaults to be used
             when prompting for commit attributes.
 
     Returns:
-        subprocess.CompletedProcess: The result from running
-        git commit. Returns the git pre-commit hook results if
+        The result from running git commit. Returns the git pre-commit hook results if
         failing during hook execution.
     """
     # Run pre-commit hooks manually so that the commit will fail
     # before prompting the user for information
     hooks_path = utils.shell_stdout("git rev-parse --git-path hooks")
     pre_commit_hook = os.path.join(hooks_path, "pre-commit")
     if not no_verify and os.path.exists(pre_commit_hook):
@@ -649,15 +650,15 @@
     with tempfile.NamedTemporaryFile(mode="w+") as commit_file:
         commit_file.write(commit_msg)
         commit_file.flush()
 
         return utils.shell(f"{commit_cmd} -F {commit_file.name}", check=False)
 
 
-def lint(range="", any=False):
+def lint(range="", any=False) -> tuple[bool, CommitRange]:
     """
     Lint commits against an upstream (branch, sha, etc).
 
     Args:
         range (str, default=''): The git revision range against which linting
             happens. The special value of ":github/pr" can be used to lint
             against the remote branch of the pull request that is opened
@@ -669,16 +670,15 @@
     Raises:
         `NoGithubPullRequestFoundError`: When using ``:github/pr`` as
             the range and no pull requests are found.
         `MultipleGithubPullRequestsFoundError`: When using ``:github/pr`` as
             the range and multiple pull requests are found.
 
     Returns:
-        tuple(bool, CommitRange): A tuple of the lint result (True/False)
-        and the associated CommitRange
+        A tuple of the lint result (True/False) and the associated CommitRange
     """
     commits = CommitRange(range=range)
     if not any:
         return not commits.filter("is_valid", False), commits
     else:
         return bool(commits.filter("is_valid", True)), commits
 
@@ -687,15 +687,15 @@
     range="",
     style="default",
     tag_match=None,
     before=None,
     after=None,
     reverse=False,
     output=None,
-):
+) -> str:
     """
     Renders git logs using tidy rendering.
 
     Args:
         range (str, default=''): The git revision range over which logs are
             output. Using ":github/pr" as the range will use the base branch
             of an open github pull request as the range. No range will result
@@ -720,15 +720,15 @@
     Raises:
         `NoGithubPullRequestFoundError`: When using ``:github/pr`` as
             the range and no pull requests are found.
         `MultipleGithubPullRequestsFoundError`: When using ``:github/pr`` as
             the range and multiple pull requests are found.
 
     Returns:
-        str: The rendered tidy log.
+        The rendered tidy log.
     """
     commits = CommitRange(
         range=range,
         tag_match=tag_match,
         before=before,
         after=after,
         reverse=reverse,
@@ -749,15 +749,15 @@
     rendered = template.render(commits=commits, output=output, range=range)
 
     _output(path=output, value=rendered)
 
     return rendered
 
 
-def squash(ref, no_verify=False, allow_empty=False):
+def squash(ref, no_verify=False, allow_empty=False) -> subprocess.CompletedProcess:
     """
     Squashes all commits since the common ancestor of ref.
 
     Args:
         ref (str): The git reference to squash against. Every commit after
             the common ancestor of this reference will be squashed.
         no_verify (bool, default=False): True if ignoring
@@ -771,17 +771,16 @@
             unexpectedly fails
         `NoGithubPullRequestFoundError`: When using ``:github/pr`` as
             the range and no pull requests are found.
         `MultipleGithubPullRequestsFoundError`: When using ``:github/pr`` as
             the range and multiple pull requests are found.
 
     Returns:
-        subprocess.CompletedProcess: The commit result. The commit result
-        contains either a failed pre-commit hook result or a successful/failed
-        commit result.
+        The commit result. The commit result contains either a failed pre-commit hook result or a
+        successful/failed commit result.
     """
     ref = github.get_pull_request_base() if ref == GITHUB_PR else ref
     range = f"{ref}.."
 
     commits = CommitRange(range=range)
     if not commits:
         raise exceptions.NoSquashableCommitsError("No commits to squash")
```

### Comparing `git-tidy-1.2.0/tidy/exceptions.py` & `git_tidy-1.2.1/tidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `git-tidy-1.2.0/tidy/github.py` & `git_tidy-1.2.1/tidy/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 Utilities for accessing Github
 """
 
 import os
 
 import requests
 
-from tidy import exceptions
-from tidy import utils
-
+from tidy import exceptions, utils
 
 GITHUB_API_TOKEN_ENV_VAR = "GITHUB_API_TOKEN"
 GITHUB_USERNAME_ENV_VAR = "GITHUB_USERNAME"
 
 
 def get_org_and_repo_name():
     remote_url = utils.shell_stdout("git remote get-url origin")
```

### Comparing `git-tidy-1.2.0/tidy/utils.py` & `git_tidy-1.2.1/tidy/utils.py`

 * *Files identical despite different names*

### Comparing `git-tidy-1.2.0/PKG-INFO` & `git_tidy-1.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,69 @@
 Metadata-Version: 2.1
 Name: git-tidy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tidy git commit messages, linting, and logging
 Home-page: https://github.com/Opus10/git-tidy
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: click (>7.0)
 Requires-Dist: formaldict (>0.2.0)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: jinja2 (>2.10.3)
 Requires-Dist: packaging (>20.0)
 Requires-Dist: python-dateutil (>2.8.1)
-Requires-Dist: pyyaml (>5.1.2)
+Requires-Dist: pyyaml (>=5.1.2,<=5.3.1)
 Requires-Dist: requests (>2.22.0)
 Project-URL: Documentation, https://git-tidy.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/git-tidy
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-git-tidy
-########
+# git-tidy
 
-``git-tidy`` is a set of git extensions for:
+`git-tidy` is a set of git extensions for:
 
-1. Keeping your git logs tidy with ease. ``git tidy-commit`` guides
-   users through a structured commit with a configurable schema.
-   ``git tidy-squash`` squashes messy commits into one tidy commit.
-2. Linting a commit log. ``git tidy-lint`` verifies that commits
-   match the schema. If a user uses ``git tidy-commit``, commits
-   will *always* validate.
-3. Rendering a commit log. ``git tidy-log`` can render commits from
-   any range and can render structured commits from a configurable
-   `Jinja <https://jinja.palletsprojects.com/en/2.11.x/>`__ template.
-   Want to automatically generate release notes? ``git tidy-log`` can
-   be configured to group and render commits based on the schema.
-
-.. image:: https://raw.githubusercontent.com/jyveapp/git-tidy/master/docs/_static/tidy-commit.gif
-    :width: 600
-
-Documentation
-=============
-
-`View the git-tidy docs here
-<https://git-tidy.readthedocs.io/>`_ for a complete tutorial on using
-``git-tidy``.
-
-Installation
-============
+1. Keeping your git logs tidy with ease. `git tidy-commit` guides users through a structured commit with a configurable schema. `git tidy-squash` squashes messy commits into one tidy commit.
+2. Linting a commit log. `git tidy-lint` verifies that commits match the schema. If a user uses `git tidy-commit`, commits will *always* validate.
+3. Rendering a commit log. `git tidy-log` can render commits from any range and can render structured commits from a configurable [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) template. Want to automatically generate release notes? `git tidy-log` can be configured to group and render commits based on the schema.
 
-``git-tidy`` can be installed a number of ways. The preferred way
-on OSX is with `homebrew <brew.sh>`__ ::
+![Example](https://raw.githubusercontent.com/jyveapp/git-tidy/main/docs/static/tidy-commit.gif)
 
-    brew tap jyveapp/homebrew-tap
-    brew install git-tidy
+## Documentation
 
-If not on OSX, one can install ``git-tidy`` system-wide with
-`pipx <https://github.com/pipxproject/pipx>`__::
+[View the git-tidy docs here](https://git-tidy.readthedocs.io/) for a complete tutorial on using `git-tidy`.
+
+## Installation
+
+One can install `git-tidy` system-wide with [pipx](https://github.com/pipxproject/pipx):
 
     pipx install git-tidy
 
-``git-tidy`` can also be installed with pip. Be sure to install it system-wide
-so that ``git-tidy``'s execution is not tied to a virtual environment::
+or pip:
 
     pip3 install git-tidy
 
+**Note** `git-tidy` depends on git at a version of 2.22 or higher. OSX users can upgrade to the latest `git` version with [homebrew](brew.sh) using `brew install git`.
 
-.. note::
-
-  ``git-tidy`` depends on git at a version of 2.22 or higher. OSX
-  users can upgrade to the latest ``git`` version with
-  `homebrew <brew.sh>`__ using ``brew install git``.
+## Compatibility
 
+`git-tidy` is compatible with Python 3.8 - 3.12.
 
-Contributing Guide
-==================
+## Contributing Guide
 
-For information on setting up git-tidy for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+For information on setting up git-tidy for development and contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
 - @tomage (Tómas Árni Jónasson)
```

