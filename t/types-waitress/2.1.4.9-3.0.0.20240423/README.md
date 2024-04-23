# Comparing `tmp/types-waitress-2.1.4.9.tar.gz` & `tmp/types-waitress-3.0.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-waitress-2.1.4.9.tar", last modified: Thu Jul 20 15:17:31 2023, max compression
+gzip compressed data, was "types-waitress-3.0.0.20240423.tar", last modified: Tue Apr 23 02:19:45 2024, max compression
```

## Comparing `types-waitress-2.1.4.9.tar` & `types-waitress-3.0.0.20240423.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.302052 types-waitress-2.1.4.9/types_waitress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:17:31.000000 types-waitress-2.1.4.9/types_waitress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:31.306052 types-waitress-2.1.4.9/waitress-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 15:17:30.000000 types-waitress-2.1.4.9/waitress-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/adjustments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/buffers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/proxy_headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/receiver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/rfc7230.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/trigger.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/utilities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 15:15:13.000000 types-waitress-2.1.4.9/waitress-stubs/wasyncore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:45.592488 types-waitress-3.0.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 02:19:45.588488 types-waitress-3.0.0.20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:45.592488 types-waitress-3.0.0.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:45.588488 types-waitress-3.0.0.20240423/types_waitress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/types_waitress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/types_waitress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/types_waitress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/types_waitress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:45.588488 types-waitress-3.0.0.20240423/waitress-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/waitress-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/adjustments.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/buffers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/proxy_headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:45.000000 types-waitress-3.0.0.20240423/waitress-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/receiver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/rfc7230.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/trigger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/utilities.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-23 02:18:48.000000 types-waitress-3.0.0.20240423/waitress-stubs/wasyncore.pyi
```

### Comparing `types-waitress-2.1.4.9/CHANGELOG.md` & `types-waitress-3.0.0.20240423/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 3.0.0.20240423 (2024-04-23)
+
+Bump waitress to 3.0.* (#11803)
+
+## 2.1.4.20240421 (2024-04-21)
+
+`waitress`: stubtest-complete and update usage of Any (#11796)
+
+## 2.1.4.20240106 (2024-01-06)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
 ## 2.1.4.9 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 2.1.4.8 (2023-05-10)
```

### Comparing `types-waitress-2.1.4.9/PKG-INFO` & `types-waitress-3.0.0.20240423/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: types-waitress
-Version: 2.1.4.9
+Version: 3.0.0.20240423
 Summary: Typing stubs for waitress
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for waitress
 
-This is a PEP 561 type stub package for the `waitress` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`waitress`](https://github.com/Pylons/waitress) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`waitress`. The source for this package can be found at
+`waitress`.
+
+This version of `types-waitress` aims to provide accurate annotations
+for `waitress==3.0.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-waitress-2.1.4.9/setup.py` & `types-waitress-3.0.0.20240423/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from setuptools import setup
 
 name = "types-waitress"
 description = "Typing stubs for waitress"
 long_description = '''
 ## Typing stubs for waitress
 
-This is a PEP 561 type stub package for the `waitress` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`waitress`](https://github.com/Pylons/waitress) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`waitress`. The source for this package can be found at
+`waitress`.
+
+This version of `types-waitress` aims to provide accurate annotations
+for `waitress==3.0.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.4.9",
+      version="3.0.0.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['waitress-stubs'],
       package_data={'waitress-stubs': ['__init__.pyi', 'adjustments.pyi', 'buffers.pyi', 'channel.pyi', 'compat.pyi', 'parser.pyi', 'proxy_headers.pyi', 'receiver.pyi', 'rfc7230.pyi', 'runner.pyi', 'server.pyi', 'task.pyi', 'trigger.pyi', 'utilities.pyi', 'wasyncore.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-waitress-2.1.4.9/types_waitress.egg-info/PKG-INFO` & `types-waitress-3.0.0.20240423/types_waitress.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: types-waitress
-Version: 2.1.4.9
+Version: 3.0.0.20240423
 Summary: Typing stubs for waitress
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/waitress.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for waitress
 
-This is a PEP 561 type stub package for the `waitress` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`waitress`](https://github.com/Pylons/waitress) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`waitress`. The source for this package can be found at
+`waitress`.
+
+This version of `types-waitress` aims to provide accurate annotations
+for `waitress==3.0.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/waitress. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-waitress-2.1.4.9/types_waitress.egg-info/SOURCES.txt` & `types-waitress-3.0.0.20240423/types_waitress.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 waitress-stubs/__init__.pyi
 waitress-stubs/adjustments.pyi
 waitress-stubs/buffers.pyi
 waitress-stubs/channel.pyi
 waitress-stubs/compat.pyi
 waitress-stubs/parser.pyi
 waitress-stubs/proxy_headers.pyi
+waitress-stubs/py.typed
 waitress-stubs/receiver.pyi
 waitress-stubs/rfc7230.pyi
 waitress-stubs/runner.pyi
 waitress-stubs/server.pyi
 waitress-stubs/task.pyi
 waitress-stubs/trigger.pyi
 waitress-stubs/utilities.pyi
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/adjustments.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/adjustments.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+from _typeshed import Incomplete
 from collections.abc import Iterable, Sequence
 from socket import socket
-from typing import Any
+from typing import Final
+from typing_extensions import TypeAlias
 
-from .compat import HAS_IPV6 as HAS_IPV6, PY2 as PY2, WIN as WIN, string_types as string_types
-from .proxy_headers import PROXY_HEADERS as PROXY_HEADERS
+# Really complex, consider unpacking a TypedDict
+_AdjustmentsParams: TypeAlias = Incomplete
 
-truthy: frozenset[Any]
-KNOWN_PROXY_HEADERS: frozenset[Any]
+truthy: frozenset[str]
+KNOWN_PROXY_HEADERS: Final[frozenset[str]]
 
 def asbool(s: bool | str | int | None) -> bool: ...
 def asoctal(s: str) -> int: ...
 def aslist_cronly(value: str) -> list[str]: ...
 def aslist(value: str) -> list[str]: ...
 def asset(value: str | None) -> set[str]: ...
 def slash_fixed_str(s: str | None) -> str: ...
 def str_iftruthy(s: str | None) -> str | None: ...
 def as_socket_list(sockets: Sequence[object]) -> list[socket]: ...
 
 class _str_marker(str): ...
 class _int_marker(int): ...
-class _bool_marker: ...
 
 class Adjustments:
     host: _str_marker
     port: _int_marker
     listen: list[str]
     threads: int
     trusted_proxy: str | None
     trusted_proxy_count: int | None
     trusted_proxy_headers: set[str]
     log_untrusted_proxy_headers: bool
-    clear_untrusted_proxy_headers: _bool_marker | bool
+    clear_untrusted_proxy_headers: bool
     url_scheme: str
     url_prefix: str
     ident: str
     backlog: int
     recv_bytes: int
     send_bytes: int
     outbuf_overflow: int
@@ -51,12 +52,14 @@
     unix_socket_perms: int
     socket_options: list[tuple[int, int, int]]
     asyncore_loop_timeout: int
     asyncore_use_poll: bool
     ipv4: bool
     ipv6: bool
     sockets: list[socket]
-    def __init__(self, **kw: Any) -> None: ...
+    channel_request_lookahead: int
+    server_name: str
+    def __init__(self, **kw: _AdjustmentsParams) -> None: ...
     @classmethod
-    def parse_args(cls, argv: str) -> tuple[dict[str, Any], Any]: ...
+    def parse_args(cls, argv: str) -> tuple[dict[str, bool], list[str]]: ...
     @classmethod
     def check_sockets(cls, sockets: Iterable[socket]) -> None: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/buffers.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/buffers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+from _typeshed import ReadableBuffer
 from io import BufferedIOBase, BufferedRandom, BytesIO
-from typing import Any
-from typing_extensions import Literal
+from typing import Final, Literal, NoReturn
 
-COPY_BYTES: int
-STRBUF_LIMIT: int
+COPY_BYTES: Final = 262144
+STRBUF_LIMIT: Final = 8192
 
 class FileBasedBuffer:
     remain: int
     file: BytesIO
     def __init__(self, file: BytesIO, from_buffer: BytesIO | None = None) -> None: ...
     def __len__(self) -> int: ...
-    def __nonzero__(self) -> bool: ...
     def __bool__(self) -> Literal[True]: ...
-    def append(self, s: Any) -> None: ...
+    def append(self, s: ReadableBuffer) -> None: ...
     def get(self, numbytes: int = -1, skip: bool = False) -> bytes: ...
     def skip(self, numbytes: int, allow_prune: int = 0) -> None: ...
-    def newfile(self) -> Any: ...
+    def newfile(self) -> BufferedIOBase: ...
     def prune(self) -> None: ...
-    def getfile(self) -> Any: ...
+    def getfile(self) -> BytesIO: ...
     def close(self) -> None: ...
 
 class TempfileBasedBuffer(FileBasedBuffer):
     def __init__(self, from_buffer: BytesIO | None = None) -> None: ...
     def newfile(self) -> BufferedRandom: ...
 
 class BytesIOBasedBuffer(FileBasedBuffer):
@@ -35,24 +34,23 @@
     def __init__(self, file: BytesIO, block_size: int = 32768) -> None: ...
     remain: int
     def prepare(self, size: int | None = None) -> int: ...
     def get(self, numbytes: int = -1, skip: bool = False) -> bytes: ...
     def __iter__(self) -> ReadOnlyFileBasedBuffer: ...
     def next(self) -> bytes | None: ...
     __next__ = next
-    def append(self, s: Any) -> None: ...
+    def append(self, s: ReadableBuffer) -> NoReturn: ...
 
 class OverflowableBuffer:
     overflowed: bool
     buf: BufferedIOBase | None
     strbuf: bytes
     overflow: int
     def __init__(self, overflow: int) -> None: ...
     def __len__(self) -> int: ...
-    def __nonzero__(self) -> bool: ...
     def __bool__(self) -> bool: ...
     def append(self, s: bytes) -> None: ...
     def get(self, numbytes: int = -1, skip: bool = False) -> bytes: ...
     def skip(self, numbytes: int, allow_prune: bool = False) -> None: ...
     def prune(self) -> None: ...
     def getfile(self) -> BytesIO: ...
     def close(self) -> None: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/channel.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/channel.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-from collections.abc import Mapping, Sequence
-from socket import socket
+from collections.abc import Sequence
+from socket import _RetAddress, socket
 from threading import Condition, Lock
 
 from waitress.adjustments import Adjustments
 from waitress.buffers import OverflowableBuffer
 from waitress.parser import HTTPRequestParser
 from waitress.server import BaseWSGIServer
 from waitress.task import ErrorTask, WSGITask
 
-from . import wasyncore as wasyncore
+from . import wasyncore
+from .wasyncore import _SocketMap
 
 class ClientDisconnected(Exception): ...
 
 class HTTPChannel(wasyncore.dispatcher):
-    task_class: WSGITask
-    error_task_class: ErrorTask
-    parser_class: HTTPRequestParser
-    request: HTTPRequestParser
+    task_class: type[WSGITask]
+    error_task_class: type[ErrorTask]
+    parser_class: type[HTTPRequestParser]
+    request: HTTPRequestParser | None
     last_activity: float
     will_close: bool
     close_when_flushed: bool
     requests: Sequence[HTTPRequestParser]
     sent_continue: bool
     total_outbufs_len: int
     current_outbuf_count: int
     server: BaseWSGIServer
     adj: Adjustments
     outbufs: Sequence[OverflowableBuffer]
     creation_time: float
     sendbuf_len: int
     task_lock: Lock
     outbuf_lock: Condition
-    addr: tuple[str, int]
+    addr: _RetAddress
     def __init__(
-        self, server: BaseWSGIServer, sock: socket, addr: str, adj: Adjustments, map: Mapping[int, socket] | None = None
+        self, server: BaseWSGIServer, sock: socket, addr: _RetAddress, adj: Adjustments, map: _SocketMap | None = None
     ) -> None: ...
+    def check_client_disconnected(self) -> None: ...
     def writable(self) -> bool: ...
     def handle_write(self) -> None: ...
     def readable(self) -> bool: ...
     def handle_read(self) -> None: ...
+    def send_continue(self) -> None: ...
     def received(self, data: bytes) -> bool: ...
     connected: bool
     def handle_close(self) -> None: ...
-    def add_channel(self, map: Mapping[int, socket] | None = None) -> None: ...
-    def del_channel(self, map: Mapping[int, socket] | None = None) -> None: ...
+    def add_channel(self, map: _SocketMap | None = None) -> None: ...
+    def del_channel(self, map: _SocketMap | None = None) -> None: ...
     def write_soon(self, data: bytes) -> int: ...
     def service(self) -> None: ...
     def cancel(self) -> None: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/parser.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/parser.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections.abc import Mapping, Sequence
 from io import BytesIO
 from re import Pattern
-from typing import Any
 
 from waitress.adjustments import Adjustments
 from waitress.receiver import ChunkedReceiver, FixedStreamReceiver
 from waitress.utilities import Error
 
+def unquote_bytes_to_wsgi(bytestring: str | bytes | bytearray) -> str: ...
+
 class ParsingError(Exception): ...
 class TransferEncodingNotImplemented(Exception): ...
 
 class HTTPRequestParser:
     completed: bool
     empty: bool
     expect_continue: bool
@@ -34,10 +35,10 @@
     def parse_header(self, header_plus: bytes) -> None: ...
     def get_body_stream(self) -> BytesIO: ...
     def close(self) -> None: ...
 
 def split_uri(uri: bytes) -> tuple[str, str, bytes, str, str]: ...
 def get_header_lines(header: bytes) -> Sequence[bytes]: ...
 
-first_line_re: Pattern[Any]
+first_line_re: Pattern[str]
 
 def crack_first_line(line: str) -> tuple[bytes, bytes, bytes]: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/proxy_headers.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/proxy_headers.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from collections.abc import Callable, Mapping, Sequence
+from _typeshed.wsgi import WSGIApplication
+from collections.abc import Mapping, Sequence
 from logging import Logger
-from typing import Any, NamedTuple
+from typing import Final, NamedTuple, TypeVar
 
-from .utilities import BadRequest as BadRequest
+_T = TypeVar("_T")
 
-PROXY_HEADERS: frozenset[Any]
+PROXY_HEADERS: Final[frozenset[str]]
 
 class Forwarded(NamedTuple):
-    by: Any
-    for_: Any
-    host: Any
-    proto: Any
+    by: str
+    for_: str
+    host: str
+    proto: str
 
 class MalformedProxyHeader(Exception):
     header: str
     reason: str
     value: str
     def __init__(self, header: str, reason: str, value: str) -> None: ...
 
 def proxy_headers_middleware(
-    app: Any,
+    app: WSGIApplication,
     trusted_proxy: str | None = None,
     trusted_proxy_count: int = 1,
     trusted_proxy_headers: set[str] | None = None,
     clear_untrusted: bool = True,
     log_untrusted: bool = False,
     logger: Logger = ...,
-) -> Callable[..., Any]: ...
+) -> WSGIApplication: ...
 def parse_proxy_headers(
     environ: Mapping[str, str], trusted_proxy_count: int, trusted_proxy_headers: set[str], logger: Logger = ...
 ) -> set[str]: ...
-def strip_brackets(addr: str) -> str: ...
+def strip_brackets(addr: Sequence[_T]) -> Sequence[_T]: ...
 def clear_untrusted_headers(
     environ: Mapping[str, str], untrusted_headers: Sequence[str], log_warning: bool = False, logger: Logger = ...
 ) -> None: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/receiver.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/receiver.pyi`

 * *Files identical despite different names*

### Comparing `types-waitress-2.1.4.9/waitress-stubs/server.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/server.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,109 @@
 import sys
-from _typeshed import Incomplete
-from collections.abc import Sequence
-from socket import socket
-from typing import Any
+from _typeshed import Unused
+from _typeshed.wsgi import WSGIApplication
+from collections.abc import Callable, Sequence
+from socket import _RetAddress, socket
+from typing import Literal
 
 from waitress import wasyncore
-from waitress.adjustments import Adjustments
+from waitress.adjustments import Adjustments, _AdjustmentsParams
 from waitress.channel import HTTPChannel
 from waitress.task import Task, ThreadedTaskDispatcher
+from waitress.wasyncore import _SocketMap
 
 def create_server(
-    application: Any,
-    map: Incomplete | None = None,
+    application: WSGIApplication,
+    map: _SocketMap | None = None,
     _start: bool = True,
     _sock: socket | None = None,
     _dispatcher: ThreadedTaskDispatcher | None = None,
-    **kw: Any,
+    **kw: _AdjustmentsParams,
 ) -> MultiSocketServer | BaseWSGIServer: ...
 
 class MultiSocketServer:
-    asyncore: Any
+    asyncore = wasyncore
     adj: Adjustments
-    map: Any
+    map: _SocketMap | None
     effective_listen: Sequence[tuple[str, int]]
     task_dispatcher: ThreadedTaskDispatcher
     def __init__(
         self,
-        map: Incomplete | None = None,
+        map: _SocketMap | None = None,
         adj: Adjustments | None = None,
         effective_listen: Sequence[tuple[str, int]] | None = None,
         dispatcher: ThreadedTaskDispatcher | None = None,
+        # Can be None, but print_listen will fail
+        log_info: Callable[[str], Unused] | None = None,
     ) -> None: ...
     def print_listen(self, format_str: str) -> None: ...
     def run(self) -> None: ...
     def close(self) -> None: ...
 
 class BaseWSGIServer(wasyncore.dispatcher):
-    channel_class: HTTPChannel
+    channel_class: type[HTTPChannel]
     next_channel_cleanup: int
     socketmod: socket
-    asyncore: Any
-    sockinfo: tuple[int, int, int, tuple[str, int]]
+    asyncore = wasyncore
+    in_connection_overflow: bool
+    sockinfo: tuple[int, int, int | None, _RetAddress]
     family: int
     socktype: int
-    application: Any
+    application: WSGIApplication
     adj: Adjustments
     trigger: int
     task_dispatcher: ThreadedTaskDispatcher
     server_name: str
     active_channels: HTTPChannel
     def __init__(
         self,
-        application: Any,
-        map: Incomplete | None = None,
+        application: WSGIApplication,
+        map: _SocketMap | None = None,
         _start: bool = True,
-        _sock: Incomplete | None = None,
+        _sock: socket | None = None,
         dispatcher: ThreadedTaskDispatcher | None = None,
         adj: Adjustments | None = None,
-        sockinfo: Incomplete | None = None,
+        sockinfo: tuple[int, int, int | None, _RetAddress] | None = None,
         bind_socket: bool = True,
-        **kw: Any,
+        **kw: _AdjustmentsParams,
     ) -> None: ...
     def bind_server_socket(self) -> None: ...
-    def get_server_name(self, ip: str) -> str: ...
-    def getsockname(self) -> Any: ...
+    def getsockname(self) -> tuple[str, str]: ...
     accepting: bool
     def accept_connections(self) -> None: ...
     def add_task(self, task: Task) -> None: ...
     def readable(self) -> bool: ...
     def writable(self) -> bool: ...
     def handle_read(self) -> None: ...
     def handle_connect(self) -> None: ...
     def handle_accept(self) -> None: ...
     def run(self) -> None: ...
     def pull_trigger(self) -> None: ...
-    def set_socket_options(self, conn: Any) -> None: ...
-    def fix_addr(self, addr: Any) -> Any: ...
+    def set_socket_options(self, conn: socket) -> None: ...
+    def fix_addr(self, addr: _RetAddress) -> _RetAddress: ...
     def maintenance(self, now: int) -> None: ...
     def print_listen(self, format_str: str) -> None: ...
     def close(self) -> None: ...
 
 class TcpWSGIServer(BaseWSGIServer):
     def bind_server_socket(self) -> None: ...
-    def getsockname(self) -> tuple[str, tuple[str, int]]: ...
+    def getsockname(self) -> tuple[str, str]: ...
     def set_socket_options(self, conn: socket) -> None: ...
 
 if sys.platform != "win32":
     class UnixWSGIServer(BaseWSGIServer):
         def __init__(
             self,
-            application: Any,
-            map: Incomplete | None = ...,
-            _start: bool = ...,
-            _sock: Incomplete | None = ...,
-            dispatcher: Incomplete | None = ...,
-            adj: Adjustments | None = ...,
-            sockinfo: Incomplete | None = ...,
-            **kw: Any,
+            application: WSGIApplication,
+            map: _SocketMap | None = None,
+            _start: bool = True,
+            _sock: socket | None = None,
+            dispatcher: ThreadedTaskDispatcher | None = None,
+            adj: Adjustments | None = None,
+            sockinfo: tuple[int, int, int | None, _RetAddress] | None = None,
+            **kw: _AdjustmentsParams,
         ) -> None: ...
         def bind_server_socket(self) -> None: ...
-        def getsockname(self) -> tuple[str, tuple[str, int]]: ...
-        def fix_addr(self, addr: Any) -> tuple[str, None]: ...
-        def get_server_name(self, ip: Any) -> str: ...
+        def getsockname(self) -> tuple[str, str]: ...
+        def fix_addr(self, addr: _RetAddress) -> tuple[Literal["localhost"], None]: ...
 
-WSGIServer: TcpWSGIServer
+WSGIServer = TcpWSGIServer
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/task.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/task.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from _typeshed import Incomplete
+from _typeshed import Unused
+from _typeshed.wsgi import WSGIEnvironment
 from collections import deque
-from collections.abc import Mapping, Sequence
+from collections.abc import Callable, Mapping, Sequence
 from logging import Logger
 from threading import Condition, Lock
-from typing import Any
 
 from .channel import HTTPChannel
 from .utilities import Error
 
 rename_headers: Mapping[str, str]
-hop_by_hop: frozenset[Any]
+hop_by_hop: frozenset[str]
 
 class ThreadedTaskDispatcher:
     stop_count: int
     active_count: int
     logger: Logger
     queue_logger: Logger
-    threads: set[Any]
+    threads: set[int]
     queue: deque[Task]
     lock: Lock
     queue_cv: Condition
     thread_exit_cv: Condition
-    def start_new_thread(self, target: Any, args: Any) -> None: ...
+    def start_new_thread(self, target: Callable[[int], Unused], thread_no: int) -> None: ...
     def handler_thread(self, thread_no: int) -> None: ...
     def set_thread_count(self, count: int) -> None: ...
     def add_task(self, task: Task) -> None: ...
     def shutdown(self, cancel_pending: bool = True, timeout: int = 5) -> bool: ...
 
 class Task:
     close_on_finish: bool
@@ -43,29 +43,30 @@
     request: Error
     response_headers: Sequence[tuple[str, str]]
     version: str
     def __init__(self, channel: HTTPChannel, request: Error) -> None: ...
     def service(self) -> None: ...
     @property
     def has_body(self) -> bool: ...
+    def set_close_on_finish(self) -> None: ...
     def build_response_header(self) -> bytes: ...
     def remove_content_length_header(self) -> None: ...
     def start(self) -> None: ...
     def finish(self) -> None: ...
     def write(self, data: bytes) -> None: ...
 
 class ErrorTask(Task):
     complete: bool
     status: str
     close_on_finish: bool
-    content_length: int
+    content_length: int | None
     def execute(self) -> None: ...
 
 class WSGITask(Task):
-    environ: Incomplete | None
+    environ: WSGIEnvironment | None
     response_headers: Sequence[tuple[str, str]]
     complete: bool
     status: str
-    content_length: int
+    content_length: int | None
     close_on_finish: bool
     def execute(self) -> None: ...
-    def get_environment(self) -> Any: ...
+    def get_environment(self) -> WSGIEnvironment: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/trigger.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/trigger.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
+from _typeshed import Unused
 from collections.abc import Callable, Mapping
 from socket import socket
 from threading import Lock
-from typing_extensions import Literal
+from typing import Literal
 
-from waitress import wasyncore as wasyncore
+from waitress import wasyncore
 
 class _triggerbase:
     kind: str | None
     lock: Lock
-    thunks: Callable[[None], None]
+    thunks: list[Callable[[None], None]]
     def readable(self) -> Literal[True]: ...
     def writable(self) -> Literal[False]: ...
     def handle_connect(self) -> None: ...
     def handle_close(self) -> None: ...
     def close(self) -> None: ...
-    def pull_trigger(self, thunk: Callable[[None], object] | None = None) -> None: ...
+    def pull_trigger(self, thunk: Callable[[None], Unused] | None = None) -> None: ...
     def handle_read(self) -> None: ...
 
 if sys.platform != "win32":
     class trigger(_triggerbase, wasyncore.file_dispatcher):
         kind: str
         def __init__(self, map: Mapping[str, _triggerbase]) -> None: ...
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/utilities.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/utilities.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,55 @@
+from _typeshed import Unused
 from _typeshed.wsgi import StartResponse
-from collections.abc import Iterator, Mapping, Sequence
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from logging import Logger
 from re import Match, Pattern
-from typing import Any
 
 logger: Logger
 queue_logger: Logger
 
 def find_double_newline(s: bytes) -> int: ...
-def concat(*args: Any) -> str: ...
-def join(seq: Any, field: str = " ") -> str: ...
-def group(s: Any) -> str: ...
+def concat(*args: str) -> str: ...
+def join(seq: Iterable[str], field: str = " ") -> str: ...
+def group(s: object) -> str: ...
 
 short_days: Sequence[str]
 long_days: Sequence[str]
 short_day_reg: str
 long_day_reg: str
 daymap: Mapping[str, int]
 hms_reg: str
 months: Sequence[str]
 monmap: Mapping[str, int]
 months_reg: str
 rfc822_date: str
-rfc822_reg: Pattern[Any]
+rfc822_reg: Pattern[str]
 
-def unpack_rfc822(m: Match[Any]) -> tuple[int, int, int, int, int, int, int, int, int]: ...
+def unpack_rfc822(m: Match[str]) -> tuple[int, int, int, int, int, int, int, int, int]: ...
 
 rfc850_date: str
-rfc850_reg: Pattern[Any]
+rfc850_reg: Pattern[str]
 
-def unpack_rfc850(m: Match[Any]) -> tuple[int, int, int, int, int, int, int, int, int]: ...
+def unpack_rfc850(m: Match[str]) -> tuple[int, int, int, int, int, int, int, int, int]: ...
 
 weekdayname: Sequence[str]
 monthname: Sequence[str]
 
 def build_http_date(when: int) -> str: ...
 def parse_http_date(d: str) -> int: ...
 def undquote(value: str) -> str: ...
 def cleanup_unix_socket(path: str) -> None: ...
 
 class Error:
     code: int
     reason: str
     body: str
     def __init__(self, body: str) -> None: ...
-    def to_response(self) -> tuple[str, Sequence[tuple[str, str]], str]: ...
-    def wsgi_response(self, environ: Any, start_response: StartResponse) -> Iterator[str]: ...
+    def to_response(self, ident: str | None = None) -> tuple[str, Sequence[tuple[str, str]], str]: ...
+    def wsgi_response(self, environ: Unused, start_response: StartResponse) -> Iterator[str]: ...
 
 class BadRequest(Error):
     code: int
     reason: str
 
 class RequestHeaderFieldsTooLarge(BadRequest):
     code: int
```

### Comparing `types-waitress-2.1.4.9/waitress-stubs/wasyncore.pyi` & `types-waitress-3.0.0.20240423/waitress-stubs/wasyncore.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 import sys
-from collections.abc import Callable, Mapping
+from _typeshed import ReadableBuffer
+from collections.abc import Mapping
 from io import BytesIO
 from logging import Logger
-from socket import socket
-from typing import Any
+from socket import _RetAddress, socket
 from typing_extensions import TypeAlias
 
-from waitress import compat as compat, utilities as utilities
-
 _Socket: TypeAlias = socket
+_SocketMap: TypeAlias = Mapping[int, socket]
 
-socket_map: Mapping[int, socket]
-map: Mapping[int, socket]
+socket_map: _SocketMap
 
 class ExitNow(Exception): ...
 
 def read(obj: dispatcher) -> None: ...
 def write(obj: dispatcher) -> None: ...
 def readwrite(obj: dispatcher, flags: int) -> None: ...
-def poll(timeout: float = 0.0, map: Mapping[int, socket] | None = None) -> None: ...
-def poll2(timeout: float = 0.0, map: Mapping[int, socket] | None = None) -> None: ...
+def poll(timeout: float = 0.0, map: _SocketMap | None = None) -> None: ...
+def poll2(timeout: float = 0.0, map: _SocketMap | None = None) -> None: ...
 
 poll3 = poll2
 
-def loop(
-    timeout: float = 30.0, use_poll: bool = False, map: Mapping[int, socket] | None = None, count: int | None = None
-) -> None: ...
+def loop(timeout: float = 30.0, use_poll: bool = False, map: _SocketMap | None = None, count: int | None = None) -> None: ...
 def compact_traceback() -> tuple[tuple[str, str, str], BaseException, BaseException, str]: ...
 
 class dispatcher:
     debug: bool
     connected: bool
     accepting: bool
     connecting: bool
     closing: bool
-    addr: tuple[str, int] | None
-    ignore_log_types: frozenset[Any]
+    addr: _RetAddress | None
+    ignore_log_types: frozenset[str]
     logger: Logger
-    compact_traceback: Callable[[], tuple[tuple[str, str, str], BaseException, BaseException, str]]
-    socket: _Socket | None
-    def __init__(self, sock: _Socket | None = None, map: Mapping[int, _Socket] | None = None) -> None: ...
-    def add_channel(self, map: Mapping[int, _Socket] | None = None) -> None: ...
-    def del_channel(self, map: Mapping[int, _Socket] | None = None) -> None: ...
+    @staticmethod
+    def compact_traceback() -> tuple[tuple[str, str, str], BaseException, BaseException, str]: ...
+    socket: socket | None
+    def __init__(self, sock: _Socket | None = None, map: _SocketMap | None = None) -> None: ...
+    def add_channel(self, map: _SocketMap | None = None) -> None: ...
+    def del_channel(self, map: _SocketMap | None = None) -> None: ...
     family_and_type: tuple[int, int]
     def create_socket(self, family: int = ..., type: int = ...) -> None: ...
-    def set_socket(self, sock: _Socket, map: Mapping[int, _Socket] | None = None) -> None: ...
+    def set_socket(self, sock: _Socket, map: _SocketMap | None = None) -> None: ...
     def set_reuse_addr(self) -> None: ...
     def readable(self) -> bool: ...
     def writable(self) -> bool: ...
     def listen(self, num: int) -> None: ...
-    def bind(self, addr: tuple[str, int]) -> None: ...
-    def connect(self, address: tuple[str, int]) -> None: ...
-    def accept(self) -> tuple[_Socket, tuple[str, int]] | None: ...
+    def bind(self, addr: _RetAddress) -> None: ...
+    def connect(self, address: _RetAddress) -> None: ...
+    def accept(self) -> tuple[_Socket, _RetAddress] | None: ...
     def send(self, data: bytes, do_close: bool = True) -> int: ...
     def recv(self, buffer_size: int) -> bytes: ...
     def close(self) -> None: ...
     def log(self, message: str) -> None: ...
     def log_info(self, message: str, type: str = "info") -> None: ...
     def handle_read_event(self) -> None: ...
     def handle_connect_event(self) -> None: ...
@@ -63,38 +60,38 @@
     def handle_expt_event(self) -> None: ...
     def handle_error(self) -> None: ...
     def handle_expt(self) -> None: ...
     def handle_read(self) -> None: ...
     def handle_write(self) -> None: ...
     def handle_connect(self) -> None: ...
     def handle_accept(self) -> None: ...
-    def handle_accepted(self, sock: _Socket, addr: Any) -> None: ...
+    def handle_accepted(self, sock: _Socket, addr: _RetAddress) -> None: ...
     def handle_close(self) -> None: ...
 
 class dispatcher_with_send(dispatcher):
     out_buffer: bytes
-    def __init__(self, sock: socket | None = None, map: Mapping[int, socket] | None = None) -> None: ...
+    def __init__(self, sock: _Socket | None = None, map: _SocketMap | None = None) -> None: ...
     def initiate_send(self) -> None: ...
-    handle_write: Callable[[], None]
+    handle_write = initiate_send
     def writable(self) -> bool: ...
     def send(self, data: bytes) -> None: ...  # type: ignore[override]
 
-def close_all(map: Mapping[int, socket] | None = None, ignore_all: bool = False) -> None: ...
+def close_all(map: _SocketMap | None = None, ignore_all: bool = False) -> None: ...
 
 if sys.platform != "win32":
     class file_wrapper:
         fd: BytesIO
         def __init__(self, fd: BytesIO) -> None: ...
         def __del__(self) -> None: ...
-        def recv(self, *args: Any) -> bytes: ...
-        def send(self, *args: Any) -> bytes: ...
-        def getsockopt(self, level: int, optname: int, buflen: bool | None = ...) -> int: ...
-        read: Callable[..., bytes]
-        write: Callable[..., bytes]
+        def recv(self, length: int, /) -> bytes: ...
+        def send(self, data: ReadableBuffer, /) -> bytes: ...
+        def getsockopt(self, level: int, optname: int, buflen: bool | None = None) -> int: ...
+        read = recv
+        write = send
         def close(self) -> None: ...
         def fileno(self) -> BytesIO: ...
 
     class file_dispatcher(dispatcher):
         connected: bool
-        def __init__(self, fd: BytesIO, map: Mapping[int, _Socket] | None = ...) -> None: ...
-        socket: _Socket
+        def __init__(self, fd: BytesIO, map: _SocketMap | None = None) -> None: ...
+        socket: socket
         def set_file(self, fd: BytesIO) -> None: ...
```

