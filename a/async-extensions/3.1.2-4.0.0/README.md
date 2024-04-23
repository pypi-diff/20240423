# Comparing `tmp/async_extensions-3.1.2.tar.gz` & `tmp/async_extensions-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-3.1.2.tar", max compression
+gzip compressed data, was "async_extensions-4.0.0.tar", max compression
```

## Comparing `async_extensions-3.1.2.tar` & `async_extensions-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1092 2024-03-21 16:13:42.662352 async_extensions-3.1.2/LICENSE
--rw-r--r--   0        0        0     2728 2024-03-21 16:13:42.662352 async_extensions-3.1.2/README.md
--rw-r--r--   0        0        0     4075 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/__init__.py
--rw-r--r--   0        0        0      740 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/blocking.py
--rw-r--r--   0        0        0      528 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/cancellation.py
--rw-r--r--   0        0        0     1053 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/channels.py
--rw-r--r--   0        0        0     6508 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/collecting.py
--rw-r--r--   0        0        0     1529 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/completion.py
--rw-r--r--   0        0        0       80 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/current.py
--rw-r--r--   0        0        0      167 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/defaults.py
--rw-r--r--   0        0        0       88 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/files.py
--rw-r--r--   0        0        0      159 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/from_thread.py
--rw-r--r--   0        0        0      174 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/paths.py
--rw-r--r--   0        0        0      128 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/processes.py
--rw-r--r--   0        0        0        0 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/py.typed
--rw-r--r--   0        0        0      269 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/resources.py
--rw-r--r--   0        0        0      439 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/results.py
--rw-r--r--   0        0        0      368 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/runners.py
--rw-r--r--   0        0        0       76 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/signals.py
--rw-r--r--   0        0        0       77 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/sleeping.py
--rw-r--r--   0        0        0     3392 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/synchronization.py
--rw-r--r--   0        0        0     1189 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/tagged.py
--rw-r--r--   0        0        0      114 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/task_groups.py
--rw-r--r--   0        0        0      120 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/task_statuses.py
--rw-r--r--   0        0        0      238 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/types.py
--rw-r--r--   0        0        0      578 2024-03-21 16:13:42.662352 async_extensions-3.1.2/async_extensions/waiting.py
--rw-r--r--   0        0        0     1872 2024-03-21 16:13:42.662352 async_extensions-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 async_extensions-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-23 12:40:02.712264 async_extensions-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2728 2024-04-23 12:40:02.712264 async_extensions-4.0.0/README.md
+-rw-r--r--   0        0        0     4075 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/blocking.py
+-rw-r--r--   0        0        0      528 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/cancellation.py
+-rw-r--r--   0        0        0     1053 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/channels.py
+-rw-r--r--   0        0        0     6508 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/collecting.py
+-rw-r--r--   0        0        0     1529 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/completion.py
+-rw-r--r--   0        0        0       80 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/current.py
+-rw-r--r--   0        0        0      167 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/defaults.py
+-rw-r--r--   0        0        0       88 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/files.py
+-rw-r--r--   0        0        0      159 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/from_thread.py
+-rw-r--r--   0        0        0      174 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/paths.py
+-rw-r--r--   0        0        0      128 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/processes.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/py.typed
+-rw-r--r--   0        0        0      269 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/resources.py
+-rw-r--r--   0        0        0      450 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/results.py
+-rw-r--r--   0        0        0      368 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/runners.py
+-rw-r--r--   0        0        0       76 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/signals.py
+-rw-r--r--   0        0        0       77 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/sleeping.py
+-rw-r--r--   0        0        0     3392 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/synchronization.py
+-rw-r--r--   0        0        0     1200 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/tagged.py
+-rw-r--r--   0        0        0      114 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/task_groups.py
+-rw-r--r--   0        0        0      120 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/task_statuses.py
+-rw-r--r--   0        0        0      238 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/types.py
+-rw-r--r--   0        0        0      597 2024-04-23 12:40:02.712264 async_extensions-4.0.0/async_extensions/waiting.py
+-rw-r--r--   0        0        0     1874 2024-04-23 12:40:02.716264 async_extensions-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 async_extensions-4.0.0/PKG-INFO
```

### Comparing `async_extensions-3.1.2/LICENSE` & `async_extensions-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/README.md` & `async_extensions-4.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^3.1.2"
+async-extensions = "^4.0.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-3.1.2/async_extensions/__init__.py` & `async_extensions-4.0.0/async_extensions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "3.1.2"
+__version__ = "4.0.0"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancellation import CancelScope, create_cancel_scope, shield
 from async_extensions.channels import (
     MemoryChannel,
     MemoryChannelFactory,
     MemoryReceiveStream,
```

### Comparing `async_extensions-3.1.2/async_extensions/blocking.py` & `async_extensions-4.0.0/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/cancellation.py` & `async_extensions-4.0.0/async_extensions/cancellation.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/channels.py` & `async_extensions-4.0.0/async_extensions/channels.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/collecting.py` & `async_extensions-4.0.0/async_extensions/collecting.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/completion.py` & `async_extensions-4.0.0/async_extensions/completion.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/standard.py` & `async_extensions-4.0.0/async_extensions/standard.py`

 * *Files identical despite different names*

### Comparing `async_extensions-3.1.2/async_extensions/tagged.py` & `async_extensions-4.0.0/async_extensions/tagged.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Awaitable, Generic, TypeVar, final
 
 from attrs import frozen
 from typing_aliases import NormalError
-from wraps.result import Result
+from wraps.primitives.result import Result
 
 from async_extensions.channels import MemoryReceiveStream, MemorySendStream
 from async_extensions.results import normal_result_of
 
 __all__ = ("TaggedResult", "NormalTaggedResult", "normal_tagged_result_of")
 
 T = TypeVar("T", covariant=True)
```

### Comparing `async_extensions-3.1.2/async_extensions/waiting.py` & `async_extensions-4.0.0/async_extensions/waiting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Awaitable, Optional, TypeVar
 
 from anyio import fail_after, move_on_after
-from wraps.option import NULL, Option, Some
-from wraps.wraps import wrap_future_option
+from wraps.primitives.option import NULL, Option, Some
+from wraps.wraps.futures import wrap_future_option
 
 from async_extensions.defaults import DEFAULT_SHIELD
 
 __all__ = ("fail_after", "move_on_after", "wait_for")
 
 T = TypeVar("T")
```

### Comparing `async_extensions-3.1.2/pyproject.toml` & `async_extensions-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "3.1.2"
+version = "4.0.0"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -31,49 +31,49 @@
 [tool.poetry.dependencies]
 python = ">= 3.8"
 
 attrs = ">= 23.2.0"
 
 anyio = ">= 4.3.0"
 solus = ">= 1.2.2"
-funcs = ">= 0.9.2"
-wraps = ">= 0.9.2"
+funcs = ">= 0.10.1"
+wraps = ">= 0.10.0"
 
 named = ">= 1.4.2"
 
 sniffio = ">= 1.3.1"
 
-typing-aliases = ">= 1.10.0"
-typing-extensions = ">= 4.10.0"
+typing-aliases = ">= 1.10.1"
+typing-extensions = ">= 4.11.0"
 
 [tool.poetry.group.format.dependencies]
-ruff = "0.3.3"
+ruff = "0.4.1"
 
 [tool.poetry.group.check.dependencies]
 mypy = "1.9.0"
 
 [tool.poetry.group.check.dependencies.pre-commit]
-version = "3.6.2"
+version = "3.7.0"
 python = ">= 3.9"
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
-changelogging = "1.4.2"
+changelogging = "1.4.1"
 
 [tool.ruff]
 line-length = 100
 
 [tool.mypy]
 strict = true
 
 [tool.changelogging]
 name = "async-extensions"
-version = "3.1.2"
+version = "4.0.0"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `async_extensions-3.1.2/PKG-INFO` & `async_extensions-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-extensions
-Version: 3.1.2
+Version: 4.0.0
 Summary: Asynchronous extensions.
 Home-page: https://github.com/nekitdev/async-extensions
 License: MIT
 Keywords: python,async,extensions
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,21 +17,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: anyio (>=4.3.0)
 Requires-Dist: attrs (>=23.2.0)
-Requires-Dist: funcs (>=0.9.2)
+Requires-Dist: funcs (>=0.10.1)
 Requires-Dist: named (>=1.4.2)
 Requires-Dist: sniffio (>=1.3.1)
 Requires-Dist: solus (>=1.2.2)
-Requires-Dist: typing-aliases (>=1.10.0)
-Requires-Dist: typing-extensions (>=4.10.0)
-Requires-Dist: wraps (>=0.9.2)
+Requires-Dist: typing-aliases (>=1.10.1)
+Requires-Dist: typing-extensions (>=4.11.0)
+Requires-Dist: wraps (>=0.10.0)
 Project-URL: Chat, https://nekit.dev/chat
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/async-extensions/issues
 Project-URL: Repository, https://github.com/nekitdev/async-extensions
 Description-Content-Type: text/markdown
 
 # `async-extensions`
@@ -75,15 +75,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^3.1.2"
+async-extensions = "^4.0.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

