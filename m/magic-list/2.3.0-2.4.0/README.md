# Comparing `tmp/magic_list-2.3.0.tar.gz` & `tmp/magic_list-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_list-2.3.0.tar", last modified: Mon Apr 22 09:01:16 2024, max compression
+gzip compressed data, was "magic_list-2.4.0.tar", last modified: Tue Apr 23 20:54:40 2024, max compression
```

## Comparing `magic_list-2.3.0.tar` & `magic_list-2.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:01:16.210511 magic_list-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 09:01:01.000000 magic_list-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-22 09:01:16.210511 magic_list-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-22 09:01:01.000000 magic_list-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:01:16.210511 magic_list-2.3.0/magic_list/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 09:01:01.000000 magic_list-2.3.0/magic_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27593 2024-04-22 09:01:01.000000 magic_list-2.3.0/magic_list/prelude.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-22 09:01:01.000000 magic_list-2.3.0/magic_list/prelude.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:01:01.000000 magic_list-2.3.0/magic_list/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:01:16.210511 magic_list-2.3.0/magic_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-22 09:01:16.000000 magic_list-2.3.0/magic_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-22 09:01:16.000000 magic_list-2.3.0/magic_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:01:16.000000 magic_list-2.3.0/magic_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 09:01:16.000000 magic_list-2.3.0/magic_list.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 09:01:16.000000 magic_list-2.3.0/magic_list.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-22 09:01:01.000000 magic_list-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:01:16.210511 magic_list-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:54:40.496883 magic_list-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 20:54:21.000000 magic_list-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-23 20:54:40.492883 magic_list-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-23 20:54:21.000000 magic_list-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:54:40.492883 magic_list-2.4.0/magic_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 20:54:21.000000 magic_list-2.4.0/magic_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-23 20:54:21.000000 magic_list-2.4.0/magic_list/prelude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-23 20:54:21.000000 magic_list-2.4.0/magic_list/prelude.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:54:21.000000 magic_list-2.4.0/magic_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:54:40.492883 magic_list-2.4.0/magic_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-23 20:54:40.000000 magic_list-2.4.0/magic_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 20:54:40.000000 magic_list-2.4.0/magic_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:54:40.000000 magic_list-2.4.0/magic_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 20:54:40.000000 magic_list-2.4.0/magic_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 20:54:40.000000 magic_list-2.4.0/magic_list.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 20:54:21.000000 magic_list-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:54:40.496883 magic_list-2.4.0/setup.cfg
```

### Comparing `magic_list-2.3.0/LICENSE` & `magic_list-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_list-2.3.0/README.md` & `magic_list-2.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
+![Logo](./docs/magic_list_banner.png)
+
 [![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
 
 [![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
 [![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
 [![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
+[![Ruff](https://github.com/qexat/magic-list/actions/workflows/ruff.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
+[![Typechecking](https://github.com/qexat/magic-list/actions/workflows/typechecking.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 Magic List is a module that extends the built-in list type.
 
-[Documentation](https://qexat.github.io/magic-list/) · [PyPI package](https://pypi.org/project/magic-list/) · [How to install](#installation)
+[Documentation](https://qexat.github.io/magic-list/) · [PyPI package](https://pypi.org/project/magic-list/) · [How to install](#installation) · [Notes for contributors and maintainers](./README-dev.md)
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
-> test coverage of 100%. It also provides typing stub files.
+> test coverage of 100%. It also provides type stubs.
 
 ## Installation
 
 ```sh
 pip install magic-list
 ```
 
 ## Examples
 
 ### Fibonacci sequence
 
-In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
+Let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
 For example, `fibonacci_sequence(10)` would return `[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55]`.
 
 ```py
 import operator
 
 from magic_list import L, list
@@ -44,9 +48,19 @@
     # the sequence
     def next_member(current: list[int]) -> int:
         return current.take_right(2).sum()
 
     return base.fill_right(next_member, n - 1)
 ```
 
-> [!NOTE]\
+> [!NOTE]
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
+
+## Contributing
+
+First of all, thank you for taking your time to participate in this project! 💕
+
+You might want to check those:
+
+- [Code of Conduct](./CODE_OF_CONDUCT.md) · a document to set standards for respectful and inclusive behavior within the community
+- [README-dev.md](./README-dev.md) · documentation to help you familiarize with Magic List's workflow
+- [Feature proposals](https://github.com/qexat/magic-list/issues/50) · a list of the proposed features in the past, present and future
```

### Comparing `magic_list-2.3.0/magic_list/prelude.py` & `magic_list-2.4.0/magic_list/prelude.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,21 +148,16 @@
         [5, 2, 3]
         >>> L[3, 5, 2].shuffled()
         [2, 5, 3]
         >>> list().shuffled()
         []
         """
 
-        result = self.__class__()
-
-        while len(result) != len(self):
-            item = random.choice(self)
-
-            if item not in result:
-                result.append(item)
+        result = self.copy()
+        random.shuffle(result)
 
         return result
 
     def map(self, function: collections.abc.Callable[[_T], _U]) -> list[_U]:
         """
         Apply `function` on each item of the list.
 
@@ -536,14 +531,58 @@
         if not hasattr(self[0], "__truediv__"):
             raise TypeError(
                 f"cannot calculate mean of list of {self[0].__class__.__name__}",
             )
 
         return sum(self) / len(self)
 
+    def min(self: list[int] | list[float]) -> int | float:
+        """
+        Return the minimum value of the list.
+
+        .. warning:: The list must be non-empty and contain numbers.
+
+        >>> L[3, 5, 2].min()
+        2
+        >>> L["hello", "world"].min()
+        *- TypeError: list of str has no minimum -*
+        >>> list().min()
+        *- TypeError: empty list has no minimum -*
+        """
+
+        if not self:
+            raise TypeError("empty list has no minimum")
+
+        if not isinstance(self.head, (int, float)):  # pyright: ignore[reportUnnecessaryIsInstance]
+            raise TypeError(f"list of {type(self.head).__name__} has no minimum")
+
+        return min(self)
+
+    def max(self: list[int] | list[float]) -> int | float:
+        """
+        Return the maximum value of the list.
+
+        .. warning:: The list must be non-empty and contain numbers.
+
+        >>> L[3, 5, 2].max()
+        2
+        >>> L["hello", "world"].max()
+        *- TypeError: list of str has no maximum -*
+        >>> list().max()
+        *- TypeError: empty list has no maximum -*
+        """
+
+        if not self:
+            raise TypeError("empty list has no maximum")
+
+        if not isinstance(self.head, (int, float)):  # pyright: ignore[reportUnnecessaryIsInstance]
+            raise TypeError(f"list of {type(self.head).__name__} has no maximum")
+
+        return max(self)
+
     def fill_left(
         self,
         filler: _T | collections.abc.Callable[[list[_T]], _T],
         n: int,
     ) -> typing_extensions.Self:
         """
         Fill on the left the list with `filler` and return the result.
```

### Comparing `magic_list-2.3.0/magic_list/prelude.pyi` & `magic_list-2.4.0/magic_list/prelude.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,22 @@
     def mean(self: list[int]) -> float: ...
     @typing.overload
     def mean(self: list[float]) -> float: ...
     @typing.overload
     def mean(self: list[complex]) -> complex: ...
     @typing.overload
     def mean(self) -> typing_extensions.Never: ...
+    @typing.overload
+    def min[NumberT: int | float | complex](self: list[NumberT]) -> NumberT: ...
+    @typing.overload
+    def min(self) -> typing_extensions.Never: ...
+    @typing.overload
+    def max[NumberT: int | float](self: list[NumberT]) -> NumberT: ...
+    @typing.overload
+    def max(self) -> typing_extensions.Never: ...
     # *- expansion-based HOFs -* #
     @typing.overload
     def fill_left(self, filler: _T, n: int) -> typing_extensions.Self: ...
     @typing.overload
     def fill_left(
         self,
         filler: _collections_abc.Callable[[list[_T]], _T],
```

### Comparing `magic_list-2.3.0/pyproject.toml` & `magic_list-2.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "magic-list"
 description = "Magic List is a module that extends the built-in list type."
-version = "2.3.0"
+version = "2.4.0"
 keywords = ["collections", "list", "built-in", "extension"]
 
 authors = [{ name = "Qexat", email = "contact@qexat.com" }]
 
 requires-python = ">=3.9"
 
 readme = "README.md"
@@ -23,18 +23,21 @@
 
 [project.urls]
 documentation = "https://qexat.github.io/magic-list/"
 repository = "https://github.com/qexat/magic-list"
 
 [project.optional-dependencies]
 dev = [
-    "build==1.2.*",
-    "coverage==7.4.*",
-    "pdoc==14.4.*",
+    "build>=1.2,<2.0",
+    "coverage>=7.4,<8.0",
+    "pdoc>=14.4,<15.0",
+    "pre-commit>=3.7,<4.0",
     "pytest>=7.4,<8.2",
-    "pyright==1.1.*",
-    "twine==5.0.*",
+    "pyright>=1.1,<2.0",
+    "ruff>=0.4,<1.0",
+    "twine>=5.0,<6.0",
+    "typing-extensions>=4.11",
 ]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

