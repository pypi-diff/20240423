# Comparing `tmp/env_star-2.4.2.tar.gz` & `tmp/env_star-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_star-2.4.2.tar", max compression
+gzip compressed data, was "env_star-2.4.3.tar", max compression
```

## Comparing `env_star-2.4.2.tar` & `env_star-2.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2024-03-28 22:21:02.195056 env_star-2.4.2/LICENSE
--rw-r--r--   0        0        0      280 2024-03-28 22:21:02.195056 env_star-2.4.2/README.md
--rw-r--r--   0        0        0      634 2024-04-23 15:49:00.171295 env_star-2.4.2/config/__init__.py
--rw-r--r--   0        0        0     1531 2024-04-23 11:14:37.970983 env_star-2.4.2/config/_helpers.py
--rw-r--r--   0        0        0     8369 2024-04-23 11:26:38.348747 env_star-2.4.2/config/config.py
--rw-r--r--   0        0        0     2258 2024-03-28 22:21:02.195056 env_star-2.4.2/config/enums.py
--rw-r--r--   0        0        0     4756 2024-03-28 22:21:02.195056 env_star-2.4.2/config/envconfig.py
--rw-r--r--   0        0        0     1409 2024-03-28 22:21:02.195056 env_star-2.4.2/config/exceptions.py
--rw-r--r--   0        0        0      926 2024-03-28 22:21:02.195056 env_star-2.4.2/config/interface.py
--rw-r--r--   0        0        0        0 2024-03-28 22:21:02.195056 env_star-2.4.2/config/py.typed
--rw-r--r--   0        0        0     6389 2024-04-23 15:48:18.226932 env_star-2.4.2/config/utils.py
--rw-r--r--   0        0        0     1303 2024-04-23 15:49:00.181295 env_star-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 env_star-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-28 22:21:02.195056 env_star-2.4.3/LICENSE
+-rw-r--r--   0        0        0      280 2024-03-28 22:21:02.195056 env_star-2.4.3/README.md
+-rw-r--r--   0        0        0      634 2024-04-23 15:54:53.113293 env_star-2.4.3/config/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-23 11:14:37.970983 env_star-2.4.3/config/_helpers.py
+-rw-r--r--   0        0        0     8369 2024-04-23 11:26:38.348747 env_star-2.4.3/config/config.py
+-rw-r--r--   0        0        0     2258 2024-03-28 22:21:02.195056 env_star-2.4.3/config/enums.py
+-rw-r--r--   0        0        0     4756 2024-03-28 22:21:02.195056 env_star-2.4.3/config/envconfig.py
+-rw-r--r--   0        0        0     1409 2024-03-28 22:21:02.195056 env_star-2.4.3/config/exceptions.py
+-rw-r--r--   0        0        0      926 2024-03-28 22:21:02.195056 env_star-2.4.3/config/interface.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:21:02.195056 env_star-2.4.3/config/py.typed
+-rw-r--r--   0        0        0     6539 2024-04-23 15:54:17.465751 env_star-2.4.3/config/utils.py
+-rw-r--r--   0        0        0     1303 2024-04-23 15:54:53.119960 env_star-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 env_star-2.4.3/PKG-INFO
```

### Comparing `env_star-2.4.2/LICENSE` & `env_star-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/__init__.py` & `env_star-2.4.3/config/__init__.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/_helpers.py` & `env_star-2.4.3/config/_helpers.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/config.py` & `env_star-2.4.3/config/config.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/enums.py` & `env_star-2.4.3/config/enums.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/envconfig.py` & `env_star-2.4.3/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/exceptions.py` & `env_star-2.4.3/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/interface.py` & `env_star-2.4.3/config/interface.py`

 * *Files identical despite different names*

### Comparing `env_star-2.4.2/config/utils.py` & `env_star-2.4.3/config/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,21 @@
 
 
 class ArgTuple(NamedTuple):
     arg: str
     cast: type
 
 
+def _try_cast(cast: Callable[[str], T], val: str) -> T | str:
+    try:
+        return cast(val)
+    except Exception:
+        return val
+
+
 def literal_cast(literal_decl: Any):
     """
     Converts a value to one of the literals defined in the provided literal declaration.
 
     Args:
         literal_decl (Any): The literal declaration, typically a `Literal` type annotation.
 
@@ -210,15 +217,15 @@
     """
     if not isinstance(literal_decl, LiteralType):
         raise TypeError
     arg_map = tuple(ArgTuple(arg, type(arg)) for arg in literal_decl.__args__)
 
     def _cast(val: str) -> Any:
         for arg, cast in arg_map:
-            if cast(val) == arg:
+            if _try_cast(cast, val) == arg:
                 return arg
         else:
             raise InvalidCast(
                 "Value received does not match any argument from literal",
                 literal_decl.__args__,
             )
```

### Comparing `env_star-2.4.2/pyproject.toml` & `env_star-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 line_length = 79
 
 [tool.black]
 line_length = 79
 
 [tool.poetry]
 name = "env-star"
-version = "2.4.2"
+version = "2.4.3"
 description = "a minimalist config manager"
 authors = ["Gustavo Correa <self.gustavocardoso@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gustcorrea/env-vars"
 packages = [{ include = "config" }]
 license = "MIT"
 classifiers = [
```

### Comparing `env_star-2.4.2/PKG-INFO` & `env_star-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-star
-Version: 2.4.2
+Version: 2.4.3
 Summary: a minimalist config manager
 Home-page: https://github.com/gustcorrea/env-vars
 License: MIT
 Author: Gustavo Correa
 Author-email: self.gustavocardoso@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

