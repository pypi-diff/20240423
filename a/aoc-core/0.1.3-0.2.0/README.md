# Comparing `tmp/aoc_core-0.1.3.tar.gz` & `tmp/aoc_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoc_core-0.1.3.tar", max compression
+gzip compressed data, was "aoc_core-0.2.0.tar", max compression
```

## Comparing `aoc_core-0.1.3.tar` & `aoc_core-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1092 2024-04-06 20:24:17.613934 aoc_core-0.1.3/LICENSE
--rw-r--r--   0        0        0     7799 2024-04-06 20:24:17.613934 aoc_core-0.1.3/README.md
--rw-r--r--   0        0        0     1607 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/__init__.py
--rw-r--r--   0        0        0       92 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/__main__.py
--rw-r--r--   0        0        0     2711 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/constants.py
--rw-r--r--   0        0        0     1898 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/data.py
--rw-r--r--   0        0        0     1241 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/errors.py
--rw-r--r--   0        0        0      107 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/__init__.py
--rw-r--r--   0        0        0      513 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/constants.py
--rw-r--r--   0        0        0     1162 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/ext/splits.py
--rw-r--r--   0        0        0     6919 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/http.py
--rw-r--r--   0        0        0    13633 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/main.py
--rw-r--r--   0        0        0     2575 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/names.py
--rw-r--r--   0        0        0     1842 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/primitives.py
--rw-r--r--   0        0        0     2675 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/runners.py
--rw-r--r--   0        0        0     5463 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/solutions.py
--rw-r--r--   0        0        0     2681 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/states.py
--rw-r--r--   0        0        0      664 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/time.py
--rw-r--r--   0        0        0     2260 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/timers.py
--rw-r--r--   0        0        0     1479 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/tokens.py
--rw-r--r--   0        0        0      289 2024-04-06 20:24:17.613934 aoc_core-0.1.3/aoc/versions.py
--rw-r--r--   0        0        0     2998 2024-04-06 20:24:17.617934 aoc_core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9423 1970-01-01 00:00:00.000000 aoc_core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-23 12:57:42.581061 aoc_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7918 2024-04-23 12:57:42.581061 aoc_core-0.2.0/README.md
+-rw-r--r--   0        0        0     1605 2024-04-23 12:57:42.581061 aoc_core-0.2.0/aoc/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/__main__.py
+-rw-r--r--   0        0        0     2711 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/constants.py
+-rw-r--r--   0        0        0     1898 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/data.py
+-rw-r--r--   0        0        0     1237 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/errors.py
+-rw-r--r--   0        0        0      107 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/ext/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/ext/constants.py
+-rw-r--r--   0        0        0     1162 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/ext/splits.py
+-rw-r--r--   0        0        0     6919 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/http.py
+-rw-r--r--   0        0        0    13640 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/main.py
+-rw-r--r--   0        0        0     2572 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/names.py
+-rw-r--r--   0        0        0     1842 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/primitives.py
+-rw-r--r--   0        0        0     2675 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/runners.py
+-rw-r--r--   0        0        0     5463 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/solutions.py
+-rw-r--r--   0        0        0     2681 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/states.py
+-rw-r--r--   0        0        0      664 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/time.py
+-rw-r--r--   0        0        0     2260 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/timers.py
+-rw-r--r--   0        0        0     1479 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/tokens.py
+-rw-r--r--   0        0        0      289 2024-04-23 12:57:42.585061 aoc_core-0.2.0/aoc/versions.py
+-rw-r--r--   0        0        0     3001 2024-04-23 12:57:42.585061 aoc_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9545 1970-01-01 00:00:00.000000 aoc_core-0.2.0/PKG-INFO
```

### Comparing `aoc_core-0.1.3/LICENSE` & `aoc_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/README.md` & `aoc_core-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add aoc-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-aoc-core = "^0.1.3"
+aoc-core = "^0.2.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.aoc-core]
 git = "https://github.com/nekitdev/aoc-core.git"
@@ -59,14 +59,16 @@
 `aoc-core` provides an extra `ext`, which installs modules like [`iters`][iters], [`funcs`][funcs]
 and [`wraps`][wraps] which can help solving problems in functional style.
 
 ## Example
 
 This example assumes `aoc` is installed and in `PATH`.
 
+One also needs to install the `ext` extra to use the `iters` module.
+
 We will be solving problem the first ever problem of Advent of Code, that is, [`2015-01`][2015-01].
 
 Firstly, we need to make sure we have the token configured:
 
 ```console
 $ aoc token print
 token not found (path `/home/nekit/.aoc`)
@@ -191,14 +193,16 @@
 Now onto part two! We need to find the first position where the floor is `-1`.
 
 Nothing too difficult, here is the solution for part two included:
 
 ```python
 from typing import Final
 
+from iters.iters import iter
+
 from aoc.solutions import Solution
 
 UP: Final = "("
 DOWN: Final = ")"
 
 NEVER_REACHED_BASEMENT: Final = "the basement was never reached"
 
@@ -212,15 +216,15 @@
 
     def solve_two(self, input: str) -> int:
         up = UP
         down = DOWN
 
         floor = 0
 
-        for position, character in enumerate(input, 1):  # one-based indexing
+        for position, character in iter(input).enumerate_from(1).unwrap():  # one-based indexing
             if character == up:
                 floor += 1
 
             if character == down:
                 floor -= 1
 
             if floor < 0:
```

### Comparing `aoc_core-0.1.3/aoc/__init__.py` & `aoc_core-0.2.0/aoc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 __description__ = "Advent of Code in Python."
 __url__ = "https://github.com/nekitdev/aoc-core"
 
 __title__ = "aoc"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 from aoc.data import dump_data, get_path_for_key, load_data
-from aoc.errors import DataNotFound, InternalError, TokenNotFound
+from aoc.errors import DataNotFound, LogicalError, TokenNotFound
 from aoc.http import HTTPClient, Route
 from aoc.names import get_key_by_name, get_name_by_key
 from aoc.primitives import Day, Key, Year
 from aoc.runners import Results, Runner, run_path
 from aoc.solutions import FinalResult, FinalSolution, Result, Solution
 from aoc.states import State
 from aoc.time import AOC_TIMEZONE, aoc_today, get_key_for_date
@@ -42,15 +42,15 @@
     "Key",
     # names
     "get_key_by_name",
     "get_name_by_key",
     # errors
     "TokenNotFound",
     "DataNotFound",
-    "InternalError",
+    "LogicalError",
     # tokens
     "load_token",
     "dump_token",
     "remove_token",
     # data
     "get_path_for_key",
     "load_data",
```

### Comparing `aoc_core-0.1.3/aoc/constants.py` & `aoc_core-0.2.0/aoc/constants.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/data.py` & `aoc_core-0.2.0/aoc/data.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/errors.py` & `aoc_core-0.2.0/aoc/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from aoc.primitives import Key
 
 __all__ = (
     # normal errors
     "TokenNotFound",
     "DataNotFound",
-    # internal errors
-    "InternalError",
+    # logical errors
+    "LogicalError",
 )
 
 TOKEN_NOT_FOUND = "token not found (path `{}`)"
 token_not_found = TOKEN_NOT_FOUND.format
 
 
 class TokenNotFound(RuntimeError):
@@ -48,9 +48,9 @@
 
     @property
     def path(self) -> Path:
         """The path to the problem's data file."""
         return self._path
 
 
-class InternalError(RuntimeError):
-    """Represents internal errors in the library."""
+class LogicalError(RuntimeError):
+    """Represents logical errors in the library."""
```

### Comparing `aoc_core-0.1.3/aoc/ext/constants.py` & `aoc_core-0.2.0/aoc/ext/constants.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/ext/splits.py` & `aoc_core-0.2.0/aoc/ext/splits.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/http.py` & `aoc_core-0.2.0/aoc/http.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/main.py` & `aoc_core-0.2.0/aoc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sys import exit
 from typing import TYPE_CHECKING, Tuple
 
 import click
 from aiohttp import ClientError
 from trogon import tui  # type: ignore
 from typing_aliases import DynamicTuple, NormalError
-from wraps import Panic
+from wraps.panics import Panic
 
 from aoc.constants import DATA_PATH, TOKEN_PATH
 from aoc.data import dump_data
 from aoc.errors import DataNotFound, TokenNotFound
 from aoc.http import HTTPClient
 from aoc.primitives import Day, Key, Part, Year
 from aoc.runners import Runner
```

### Comparing `aoc_core-0.1.3/aoc/names.py` & `aoc_core-0.2.0/aoc/names.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from re import compile
 from typing import Literal
 
-from aoc.errors import InternalError
+from aoc.errors import LogicalError
 from aoc.primitives import Day, Key, Year
 
 __all__ = ("get_key_by_name", "get_name_by_key")
 
 YEAR: Literal["year"] = "year"
 """The `year` literal."""
 
 DAY: Literal["day"] = "day"
 """The `day` literal."""
 
 YEAR_TITLE = YEAR.title()
 """The `Year` literal."""
+
 DAY_TITLE = DAY.title()
 """The `Day` literal."""
 
 NAME_PATTERN = rf"^{YEAR_TITLE}(?P<{YEAR}>[0-9]{{4}}){DAY_TITLE}(?P<{DAY}>[0-9]{{2}})$"
 
 NAME = compile(NAME_PATTERN)
 
@@ -44,32 +45,32 @@
 
     Returns:
         The key representing the problem.
 
     Raises:
         TypeError: The `name` does not match the expected format.
         ValueError: The year or the day is not valid.
-        InternalError: The pattern was matched but `year` or `day` group is not set.
+        LogicalError: The pattern was matched but `year` or `day` group is not set.
     """
     match = NAME.match(name)
 
     if match is None:
         raise TypeError(invalid_name(name))
 
     year_option = match.group(YEAR)
 
     if year_option is None:
-        raise InternalError(NAME_MATCHED_BUT_NO_YEAR)
+        raise LogicalError(NAME_MATCHED_BUT_NO_YEAR)
 
     year_value = int(year_option)
 
     day_option = match.group(DAY)
 
     if day_option is None:
-        raise InternalError(NAME_MATCHED_BUT_NO_DAY)
+        raise LogicalError(NAME_MATCHED_BUT_NO_DAY)
 
     day_value = int(day_option)
 
     try:
         year = Year(year_value)
 
     except ValueError as invalid_year:
```

### Comparing `aoc_core-0.1.3/aoc/primitives.py` & `aoc_core-0.2.0/aoc/primitives.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/runners.py` & `aoc_core-0.2.0/aoc/runners.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/solutions.py` & `aoc_core-0.2.0/aoc/solutions.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/states.py` & `aoc_core-0.2.0/aoc/states.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/time.py` & `aoc_core-0.2.0/aoc/time.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/timers.py` & `aoc_core-0.2.0/aoc/timers.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/aoc/tokens.py` & `aoc_core-0.2.0/aoc/tokens.py`

 * *Files identical despite different names*

### Comparing `aoc_core-0.1.3/pyproject.toml` & `aoc_core-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aoc-core"
-version = "0.1.3"
+version = "0.2.0"
 description = "Advent of Code in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/aoc-core"
@@ -37,64 +37,64 @@
 
 attrs = ">= 23.2.0"
 
 pendulum = ">= 3.0.0"
 
 click = ">= 8.1.7"
 
-versions = ">= 2.1.2"
+versions = ">= 3.0.0"
 
 entrypoint = ">= 2.0.3"
 
-aiohttp = ">= 3.9.3"
+aiohttp = ">= 3.9.5"
 yarl = ">= 1.9.4"
 
-typing-aliases = ">= 1.8.0"
-typing-extensions = ">= 4.10.0"
-wraps = ">= 0.9.2"
+typing-aliases = ">= 1.10.1"
+typing-extensions = ">= 4.11.0"
+wraps = ">= 0.10.0"
 
 [tool.poetry.dependencies.trogon]
 version = ">= 0.5.0"
 python = "^3.8"
 
 [tool.poetry.dependencies.funcs]
-version = ">= 0.9.2"
+version = ">= 0.10.1"
 optional = true
 
 [tool.poetry.dependencies.iters]
-version = ">= 0.16.2"
+version = ">= 0.18.0"
 optional = true
 
 [tool.poetry.extras]
 ext = ["funcs", "iters"]  # `wraps` is required to handle panics
 
 [tool.poetry.group.format.dependencies]
-ruff = "0.3.3"
+ruff = "0.4.1"
 
 [tool.poetry.group.check.dependencies]
 mypy = "1.9.0"
 
 [tool.poetry.group.check.dependencies.pre-commit]
-version = "3.6.2"
+version = "3.7.0"
 python = ">= 3.9"
 
 [tool.poetry.group.test.dependencies]
 coverage = "7.4.4"
 pytest = "8.1.1"
-pytest-cov = "4.1.0"
+pytest-cov = "5.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-mkdocs-material = "9.5.13"
+mkdocs-material = "9.5.18"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.24.0"
+version = "0.24.3"
 extras = ["python"]
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
 changelogging = "1.4.2"
@@ -131,15 +131,15 @@
 directory = "coverage"
 
 [tool.mypy]
 strict = true
 
 [tool.changelogging]
 name = "aoc-core"
-version = "0.1.3"
+version = "0.2.0"
 url = "https://github.com/nekitdev/aoc-core"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `aoc_core-0.1.3/PKG-INFO` & `aoc_core-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoc-core
-Version: 0.1.3
+Version: 0.2.0
 Summary: Advent of Code in Python.
 Home-page: https://github.com/nekitdev/aoc-core
 License: MIT
 Keywords: python,aoc
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
@@ -16,26 +16,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: ext
-Requires-Dist: aiohttp (>=3.9.3)
+Requires-Dist: aiohttp (>=3.9.5)
 Requires-Dist: attrs (>=23.2.0)
 Requires-Dist: click (>=8.1.7)
 Requires-Dist: entrypoint (>=2.0.3)
-Requires-Dist: funcs (>=0.9.2) ; extra == "ext"
-Requires-Dist: iters (>=0.16.2) ; extra == "ext"
+Requires-Dist: funcs (>=0.10.1) ; extra == "ext"
+Requires-Dist: iters (>=0.18.0) ; extra == "ext"
 Requires-Dist: pendulum (>=3.0.0)
 Requires-Dist: trogon (>=0.5.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: typing-aliases (>=1.8.0)
-Requires-Dist: typing-extensions (>=4.10.0)
-Requires-Dist: versions (>=2.1.2)
-Requires-Dist: wraps (>=0.9.2)
+Requires-Dist: typing-aliases (>=1.10.1)
+Requires-Dist: typing-extensions (>=4.11.0)
+Requires-Dist: versions (>=3.0.0)
+Requires-Dist: wraps (>=0.10.0)
 Requires-Dist: yarl (>=1.9.4)
 Project-URL: Chat, https://nekit.dev/chat
 Project-URL: Documentation, https://nekitdev.github.io/aoc-core
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/aoc-core/issues
 Project-URL: Repository, https://github.com/nekitdev/aoc-core
 Description-Content-Type: text/markdown
@@ -82,15 +82,15 @@
 $ poetry add aoc-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-aoc-core = "^0.1.3"
+aoc-core = "^0.2.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.aoc-core]
 git = "https://github.com/nekitdev/aoc-core.git"
@@ -101,14 +101,16 @@
 `aoc-core` provides an extra `ext`, which installs modules like [`iters`][iters], [`funcs`][funcs]
 and [`wraps`][wraps] which can help solving problems in functional style.
 
 ## Example
 
 This example assumes `aoc` is installed and in `PATH`.
 
+One also needs to install the `ext` extra to use the `iters` module.
+
 We will be solving problem the first ever problem of Advent of Code, that is, [`2015-01`][2015-01].
 
 Firstly, we need to make sure we have the token configured:
 
 ```console
 $ aoc token print
 token not found (path `/home/nekit/.aoc`)
@@ -233,14 +235,16 @@
 Now onto part two! We need to find the first position where the floor is `-1`.
 
 Nothing too difficult, here is the solution for part two included:
 
 ```python
 from typing import Final
 
+from iters.iters import iter
+
 from aoc.solutions import Solution
 
 UP: Final = "("
 DOWN: Final = ")"
 
 NEVER_REACHED_BASEMENT: Final = "the basement was never reached"
 
@@ -254,15 +258,15 @@
 
     def solve_two(self, input: str) -> int:
         up = UP
         down = DOWN
 
         floor = 0
 
-        for position, character in enumerate(input, 1):  # one-based indexing
+        for position, character in iter(input).enumerate_from(1).unwrap():  # one-based indexing
             if character == up:
                 floor += 1
 
             if character == down:
                 floor -= 1
 
             if floor < 0:
```

