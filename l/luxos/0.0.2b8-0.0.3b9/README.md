# Comparing `tmp/luxos-0.0.2b8.tar.gz` & `tmp/luxos-0.0.3b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.2b8.tar", last modified: Thu Apr 18 15:03:27 2024, max compression
+gzip compressed data, was "luxos-0.0.3b9.tar", last modified: Tue Apr 23 14:08:56 2024, max compression
```

## Comparing `luxos-0.0.2b8.tar` & `luxos-0.0.3b9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 15:03:27.204679 luxos-0.0.2b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-18 15:02:56.000000 luxos-0.0.2b8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-18 15:03:25.000000 luxos-0.0.2b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:03:27.204679 luxos-0.0.2b8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.196678 luxos-0.0.2b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 15:03:25.000000 luxos-0.0.2b8/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.200679 luxos-0.0.2b8/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-18 15:02:56.000000 luxos-0.0.2b8/src/luxos/scripts/luxos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 15:03:27.000000 luxos-0.0.2b8/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:03:27.204679 luxos-0.0.2b8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 15:02:56.000000 luxos-0.0.2b8/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.077522 luxos-0.0.3b9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-23 14:08:56.077522 luxos-0.0.3b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 14:08:24.000000 luxos-0.0.3b9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 14:08:53.000000 luxos-0.0.3b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:08:56.077522 luxos-0.0.3b9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.069522 luxos-0.0.3b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 14:08:53.000000 luxos-0.0.3b9/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/luxos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.077522 luxos-0.0.3b9/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.2b8/PKG-INFO` & `luxos-0.0.3b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.2b8
+Version: 0.0.3b9
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.2b8/README.md` & `luxos-0.0.3b9/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/pyproject.toml` & `luxos-0.0.3b9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.2b8"
+version = "0.0.3b9"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.2b8/src/luxos/api.json` & `luxos-0.0.3b9/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/api.py` & `luxos-0.0.3b9/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/asyncops.py` & `luxos-0.0.3b9/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/cli/v1.py` & `luxos-0.0.3b9/src/luxos/cli/v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     pass
 
 
 class AbortCliError(CliBaseError):
     pass
 
 
-def setup_logging(count: int, config: dict[str, Any]) -> None:
+def setup_logging(config: dict[str, Any], count: int) -> None:
     levelmap = {
         1: logging.DEBUG,
         0: logging.INFO,
         -1: logging.WARNING,
     }
 
     # we can set the default log level in LOGGING_CONFIG
@@ -169,26 +169,28 @@
 
         # setup the logging
         config = {}
         if value := self.module_variables.get("LOGGING_CONFIG"):
             config = value.copy()
 
         count = max(min((options.verbose or 0) - (options.quiet or 0), 1), -1)
-        setup_logging(count, config)
+        setup_logging(config, count)
 
         return options
 
     @classmethod
-    def get_parser(cls, module_variables):
+    def get_parser(cls, module_variables, **kwargs):
         class Formatter(
             argparse.ArgumentDefaultsHelpFormatter, argparse.RawTextHelpFormatter
         ):
             pass
 
-        return cls(module_variables=module_variables, formatter_class=Formatter)
+        return cls(
+            module_variables=module_variables, formatter_class=Formatter, **kwargs
+        )
 
 
 def cli(
     add_arguments: Callable[[argparse.ArgumentParser], None] | None = None,
     process_args: (
         Callable[[argparse.Namespace], argparse.Namespace | None] | None
     ) = None,
@@ -202,16 +204,21 @@
             module = inspect.getmodule(function)
             for name in list(module_variables):
                 module_variables[name] = getattr(module, name, None)
 
             if "args" in sig.parameters and "parser" in sig.parameters:
                 raise RuntimeError("cannot use args and parser at the same time")
 
+            description, _, epilog = (
+                (function.__doc__ or module.__doc__ or "").strip().partition("\n")
+            )
             kwargs = {}
-            parser = LuxosParser.get_parser(module_variables)
+            parser = LuxosParser.get_parser(
+                module_variables, description=description, epilog=epilog
+            )
             if add_arguments:
                 add_arguments(parser)
 
             if "parser" in sig.parameters:
                 kwargs["parser"] = parser
 
             t0 = time.monotonic()
@@ -250,7 +257,21 @@
             def _cli2(*args, **kwargs):
                 with setup() as ba:
                     return function(*ba.args, **ba.kwargs)
 
         return _cli2
 
     return _cli1
+
+
+### standard arguments
+
+
+def add_argument_csv_miners(parser: argparse.ArgumentParser, *args, **kwargs):
+    """adds arguments handling miners config in a csv file"""
+
+    parser.add_argument("--ip-start", help="start of the IP range")
+    parser.add_argument("--ip-end", help="start of the IP range")
+    parser.add_argument("--ip-file", type=Path, help="csv file containing ip addresses")
+    parser.add_argument(
+        "--port", type=int, default=4028, help="Port number for the miner API"
+    )
```

### Comparing `luxos-0.0.2b8/src/luxos/exceptions.py` & `luxos-0.0.3b9/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/misc.py` & `luxos-0.0.3b9/src/luxos/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # catch-all module (find later a better place)
 from __future__ import annotations
 import sys
 import itertools
+import ipaddress
+from typing import Generator
 
 
 if sys.version_info >= (3, 12):
     batched = itertools.batched
 else:
+
     def batched(iterable, n):
         if n < 1:
             raise ValueError("n must be at least one")
         it = iter(iterable)
         while batch := tuple(itertools.islice(it, n)):
             yield batch
 
@@ -24,8 +27,32 @@
     if txt.endswith("\n"):
         last_eol = "\n"
         txt = txt[:-1]
     else:
         last_eol = ""
 
     result = pre + txt.replace("\n", "\n" + pre) + last_eol
-    return result if result.strip() else result.strip()
+    return result if result.strip() else result.strip()
+
+
+def iter_ip_ranges(txt: str) -> Generator[str, None, None]:
+    """iterate over ip ranges
+
+    for ip in iter_ip_ranges("127.0.0.1-127.0.0.3:127.0.0.15"):
+        print(ip)
+
+    127.0.0.1
+    127.0.0.2
+    127.0.0.3
+    127.0.0.15
+    """
+
+    for segment in txt.split(":"):
+        start, _, end = segment.partition("-")
+        if not end:
+            yield start
+        else:
+            cur = ipaddress.IPv4Address(start)
+            last = ipaddress.IPv4Address(end)
+            while cur <= last:
+                yield str(cur)
+                cur += 1
```

### Comparing `luxos-0.0.2b8/src/luxos/scripts/async_luxos.py` & `luxos-0.0.3b9/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/scripts/health_checker.py` & `luxos-0.0.3b9/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos/scripts/luxos.py` & `luxos-0.0.3b9/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.3b9/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.2b8
+Version: 0.0.3b9
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.2b8/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.3b9/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/tests/test_cli.py` & `luxos-0.0.3b9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.2b8/tests/test_luxos_asyncops.py` & `luxos-0.0.3b9/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

