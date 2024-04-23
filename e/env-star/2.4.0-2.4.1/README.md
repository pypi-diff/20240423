# Comparing `tmp/env_star-2.4.0.tar.gz` & `tmp/env_star-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_star-2.4.0.tar", max compression
+gzip compressed data, was "env_star-2.4.1.tar", max compression
```

## Comparing `env_star-2.4.0.tar` & `env_star-2.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2024-03-28 22:21:02.195056 env_star-2.4.0/LICENSE
--rw-r--r--   0        0        0      280 2024-03-28 22:21:02.195056 env_star-2.4.0/README.md
--rw-r--r--   0        0        0      634 2024-03-28 22:23:02.074703 env_star-2.4.0/config/__init__.py
--rw-r--r--   0        0        0     1615 2024-03-28 22:21:02.195056 env_star-2.4.0/config/_helpers.py
--rw-r--r--   0        0        0     8527 2024-03-28 22:21:02.195056 env_star-2.4.0/config/config.py
--rw-r--r--   0        0        0     2258 2024-03-28 22:21:02.195056 env_star-2.4.0/config/enums.py
--rw-r--r--   0        0        0     4756 2024-03-28 22:21:02.195056 env_star-2.4.0/config/envconfig.py
--rw-r--r--   0        0        0     1409 2024-03-28 22:21:02.195056 env_star-2.4.0/config/exceptions.py
--rw-r--r--   0        0        0      926 2024-03-28 22:21:02.195056 env_star-2.4.0/config/interface.py
--rw-r--r--   0        0        0        0 2024-03-28 22:21:02.195056 env_star-2.4.0/config/py.typed
--rw-r--r--   0        0        0     4702 2024-03-28 22:21:02.195056 env_star-2.4.0/config/utils.py
--rw-r--r--   0        0        0     1302 2024-03-28 22:23:02.081370 env_star-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 env_star-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-28 22:21:02.195056 env_star-2.4.1/LICENSE
+-rw-r--r--   0        0        0      280 2024-03-28 22:21:02.195056 env_star-2.4.1/README.md
+-rw-r--r--   0        0        0      634 2024-04-23 11:40:17.988919 env_star-2.4.1/config/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-23 11:14:37.970983 env_star-2.4.1/config/_helpers.py
+-rw-r--r--   0        0        0     8369 2024-04-23 11:26:38.348747 env_star-2.4.1/config/config.py
+-rw-r--r--   0        0        0     2258 2024-03-28 22:21:02.195056 env_star-2.4.1/config/enums.py
+-rw-r--r--   0        0        0     4756 2024-03-28 22:21:02.195056 env_star-2.4.1/config/envconfig.py
+-rw-r--r--   0        0        0     1409 2024-03-28 22:21:02.195056 env_star-2.4.1/config/exceptions.py
+-rw-r--r--   0        0        0      926 2024-03-28 22:21:02.195056 env_star-2.4.1/config/interface.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:21:02.195056 env_star-2.4.1/config/py.typed
+-rw-r--r--   0        0        0     6389 2024-04-23 11:33:01.424844 env_star-2.4.1/config/utils.py
+-rw-r--r--   0        0        0     1303 2024-04-23 11:40:17.995586 env_star-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 env_star-2.4.1/PKG-INFO
```

### Comparing `env_star-2.4.0/LICENSE` & `env_star-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/__init__.py` & `env_star-2.4.1/config/__init__.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/_helpers.py` & `env_star-2.4.1/config/_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import contextlib
 import typing
 
-from typing_extensions import ParamSpec, Self
-
 from config.exceptions import StrictCast
 
 T = typing.TypeVar("T")
-P = ParamSpec("P")
+P = typing.ParamSpec("P")
 
 ExcT = typing.TypeVar("ExcT", bound=Exception)
 
 
 def panic(exc: type[ExcT], message: str, *excargs) -> ExcT:
     return exc(f"{message.removesuffix('!')}!", *excargs)
 
@@ -18,17 +16,15 @@
 def clean_dotenv_value(value: str) -> str:
     """clean_dotenv_value removes leading and trailing whitespace and removes
     wrapping quotes from the value."""
     # Remove leading and trailing whitespace
     value = value.strip()
 
     # Check if value has quotes at the beginning and end
-    has_quotes = (
-        len(value) >= 2 and value[0] == value[-1] and value[0] in ['"', "'"]
-    )
+    has_quotes = len(value) >= 2 and value[0] == value[-1] and value[0] in ['"', "'"]
 
     # Remove quotes if they exist (only once)
     if has_quotes:
         value = value[1:-1]
 
     return value
 
@@ -43,17 +39,13 @@
         self._func = func
 
     def strict(self, *args: P.args, **kwargs: P.kwargs) -> T:
         if (result := self._func(*args, **kwargs)) is not None:
             return result
         raise panic(StrictCast, f"received falsy value {result}", result)
 
-    def __call__(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> typing.Optional[T]:
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> typing.Optional[T]:
         return self._func(*args, **kwargs)
 
-    def optional(
-        self, *args: P.args, **kwargs: P.kwargs
-    ) -> typing.Optional[T]:
+    def optional(self, *args: P.args, **kwargs: P.kwargs) -> typing.Optional[T]:
         with contextlib.suppress(Exception):
             return self._func(*args, **kwargs)
```

### Comparing `env_star-2.4.0/config/config.py` & `env_star-2.4.1/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     MutableMapping,
     TypeVar,
     Union,
     overload,
 )
 
 from gyver.attrs import define, info
+from lazyfields import lazyfield
 
 from config._helpers import clean_dotenv_value, panic
-from lazyfields import lazyfield
-from config.exceptions import InvalidCast, InvalidEnv, MissingName
+from config.exceptions import InvalidCast, MissingName
 from config.interface import MISSING, _default_cast
 
 T = TypeVar("T")
 
 
 @define
 class EnvMapping(MutableMapping[str, str]):
@@ -55,17 +55,15 @@
             name (str): The name of the environment variable.
             value (str): The new value for the environment variable.
 
         Raises:
             KeyError: If the environment variable has already been read.
         """
         if name in self.already_read:
-            raise panic(
-                KeyError, f"{name} already read, cannot change its value"
-            )
+            raise panic(KeyError, f"{name} already read, cannot change its value")
         self.mapping[name] = value
 
     def __delitem__(self, name: str) -> None:
         """
         Delete the specified environment variable.
 
         Args:
@@ -136,17 +134,15 @@
             env_file (Union[str, Path]): The path to the environment file.
 
         Yields:
             tuple[str, str]: Pairs of environment variable names and their values.
         """
         with open(env_file, "r") as buf:
             for line in buf:
-                line = (
-                    line.strip()
-                )  # Remove leading/trailing whitespaces and newlines
+                line = line.strip()  # Remove leading/trailing whitespaces and newlines
                 if not line or line.startswith(
                     "#"
                 ):  # Skip empty lines and full-line comments
                     continue
 
                 # Handle lines with comments after the value
 
@@ -177,17 +173,15 @@
 
         Raises:
             InvalidCast: If casting the value is unsuccessful.
         """
         try:
             val = cast(val)
         except Exception as e:
-            raise panic(
-                InvalidCast, f"{name} received an invalid value {val}"
-            ) from e
+            raise panic(InvalidCast, f"{name} received an invalid value {val}") from e
         else:
             return val
 
     def _get_val(
         self, name: str, default: Union[Any, type[MISSING]] = MISSING
     ) -> Union[Any, type[MISSING]]:
         """
@@ -226,36 +220,32 @@
 
         Raises:
             MissingName: If the environment variable is not found and no default value is provided.
             InvalidCast: If casting the value is unsuccessful.
         """
         val = self._get_val(name, default)
         if val is MISSING:
-            raise panic(
-                MissingName, f"{name} not found and no default was given"
-            )
+            raise panic(MissingName, f"{name} not found and no default was given")
         return self._cast(name, val, cast)
 
     @overload
     def __call__(
         self,
         name: str,
         cast: Union[Callable[[Any], T], type[T]] = _default_cast,
         default: type[MISSING] = MISSING,
-    ) -> T:
-        ...
+    ) -> T: ...
 
     @overload
     def __call__(
         self,
         name: str,
         cast: Union[Callable[[Any], T], type[T]] = _default_cast,
         default: T = ...,
-    ) -> T:
-        ...
+    ) -> T: ...
 
     def __call__(
         self,
         name: str,
         cast: Union[Callable[[Any], T], type[T]] = _default_cast,
         default: Union[T, type[MISSING]] = MISSING,
     ) -> T:
```

### Comparing `env_star-2.4.0/config/enums.py` & `env_star-2.4.1/config/enums.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/envconfig.py` & `env_star-2.4.1/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/exceptions.py` & `env_star-2.4.1/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/interface.py` & `env_star-2.4.1/config/interface.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.0/config/utils.py` & `env_star-2.4.1/config/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from collections.abc import Callable
 from pathlib import Path
 from shlex import shlex
-from typing import Any, Callable, Generic, TypeVar, Union, overload
+from typing import Any, Generic, Literal, NamedTuple, TypeVar, Union, overload
 
 from config._helpers import maybe_result
-from config.exceptions import InvalidEnv
+from config.exceptions import InvalidCast, InvalidEnv
 
 
 @maybe_result
 def boolean_cast(string: str):
     """
     Converts a string to its boolean equivalent.
 
@@ -31,28 +32,24 @@
 
 
 T = TypeVar("T")
 
 
 @overload
 def comma_separated(
-    cast: Callable[[str], str] = str
-) -> Callable[[str], tuple[str, ...]]:
-    ...
+    cast: Callable[[str], str] = str,
+) -> Callable[[str], tuple[str, ...]]: ...
 
 
 @overload
-def comma_separated(
-    cast: Callable[[str], T]
-) -> Callable[[str], tuple[T, ...]]:
-    ...
+def comma_separated(cast: Callable[[str], T]) -> Callable[[str], tuple[T, ...]]: ...
 
 
 def comma_separated(
-    cast: Callable[[str], Union[T, str]] = str
+    cast: Callable[[str], Union[T, str]] = str,
 ) -> Callable[[str], tuple[Union[T, str], ...]]:
     """
     Converts a comma-separated string to a tuple of values after applying the given cast function.
 
     Args:
         cast (Callable[[str], Union[T, str]]): The casting function to apply to each item in the comma-separated string.
             Defaults to `str`.
@@ -98,14 +95,15 @@
 U = TypeVar("U")
 
 
 class _JoinedCast(Generic[S, T]):
     """
     A utility class for chaining casting operations.
     """
+
     def __init__(self, cast: Callable[[S], T]) -> None:
         self._cast = cast
 
     def __call__(self, val: S) -> T:
         return self._cast(val)
 
     def cast(self, cast: Callable[[T], U]) -> "_JoinedCast[S, U]":
@@ -126,14 +124,15 @@
 
         Args:
             cast (Callable): The casting function to apply.
 
         Returns:
             Callable: A new casting function that combines the existing casting function and the provided one.
         """
+
         def _wrapper(val: Any):
             return cast(self._cast(val))
 
         return _wrapper
 
 
 def joined_cast(cast: Callable[[str], T]) -> _JoinedCast[str, T]:
@@ -169,7 +168,58 @@
                 f"Value {val} did not pass rule check {rule.__name__}",
                 rule,
                 val,
             )
         return val
 
     return caster
+
+
+LiteralType = type(Literal["Any"])
+
+
+class ArgTuple(NamedTuple):
+    arg: str
+    cast: type
+
+
+def literal_cast(literal_decl: Any):
+    """
+    Converts a value to one of the literals defined in the provided literal declaration.
+
+    Args:
+        literal_decl (Any): The literal declaration, typically a `Literal` type annotation.
+
+    Returns:
+        Callable[[str], Any]: A casting function that checks if the value matches any of the literals defined
+            in the declaration. If a match is found, it returns the value as is. Otherwise, it raises an `InvalidCast`
+            exception.
+
+    Raises:
+        TypeError: If the provided literal declaration is not an instance of `Literal`.
+        InvalidCast: If the value received does not match any argument from the literal declaration.
+
+    Examples:
+        >>> literal_cast(Literal["Any"])("Any")
+        'Any'
+        >>> literal_cast(Literal[1, "two", 3.0])("3.0")
+        3.0
+        >>> literal_cast(Literal[1, "two", 3.0])("four")
+        Traceback (most recent call last):
+            ...
+        InvalidCast: Value received does not match any argument from literal: (1, 'two', 3.0)
+    """
+    if not isinstance(literal_decl, LiteralType):
+        raise TypeError
+    arg_map = tuple(ArgTuple(arg, type(arg)) for arg in literal_decl.__args__)
+
+    def _cast(val: str) -> Any:
+        for arg, cast in arg_map:
+            if cast(val) == arg:
+                return val
+        else:
+            raise InvalidCast(
+                "Value received does not match any argument from literal",
+                literal_decl.__args__,
+            )
+
+    return _cast
```

### Comparing `env_star-2.4.0/pyproject.toml` & `env_star-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 line_length = 79
 
 [tool.black]
 line_length = 79
 
 [tool.poetry]
 name = "env-star"
-version = "2.4.0"
+version = "2.4.1"
 description = "a minimalist config manager"
 authors = ["Gustavo Correa <self.gustavocardoso@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gustcorrea/env-vars"
 packages = [{ include = "config" }]
 license = "MIT"
 classifiers = [
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 typing-extensions = "^4.7.1"
 gyver-attrs = "^0.9.0"
 lazy-fields = "^1.0.1"
 
 
 [tool.poetry.group.testing.dependencies]
 pytest = "^7.4.0"
```

### Comparing `env_star-2.4.0/PKG-INFO` & `env_star-2.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: env-star
-Version: 2.4.0
+Version: 2.4.1
 Summary: a minimalist config manager
 Home-page: https://github.com/gustcorrea/env-vars
 License: MIT
 Author: Gustavo Correa
 Author-email: self.gustavocardoso@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: gyver-attrs (>=0.9.0,<0.10.0)
 Requires-Dist: lazy-fields (>=1.0.1,<2.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/gustcorrea/env-vars
 Description-Content-Type: text/markdown
 
 # env-vars
```

