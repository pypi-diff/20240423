# Comparing `tmp/types-croniter-2.0.0.20240321.tar.gz` & `tmp/types-croniter-2.0.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-croniter-2.0.0.20240321.tar", last modified: Thu Mar 21 02:15:19 2024, max compression
+gzip compressed data, was "types-croniter-2.0.0.20240423.tar", last modified: Tue Apr 23 02:19:33 2024, max compression
```

## Comparing `types-croniter-2.0.0.20240321.tar` & `types-croniter-2.0.0.20240423.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:15:19.493558 types-croniter-2.0.0.20240321/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-21 02:15:19.493558 types-croniter-2.0.0.20240321/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:15:19.489558 types-croniter-2.0.0.20240321/croniter-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/croniter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-21 02:15:01.000000 types-croniter-2.0.0.20240321/croniter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-03-21 02:15:01.000000 types-croniter-2.0.0.20240321/croniter-stubs/croniter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 02:15:19.493558 types-croniter-2.0.0.20240321/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:15:19.493558 types-croniter-2.0.0.20240321/types_croniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/types_croniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/types_croniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/types_croniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-21 02:15:19.000000 types-croniter-2.0.0.20240321/types_croniter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:33.884474 types-croniter-2.0.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 02:19:33.884474 types-croniter-2.0.0.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:33.884474 types-croniter-2.0.0.20240423/croniter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/croniter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 02:18:48.000000 types-croniter-2.0.0.20240423/croniter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-23 02:18:48.000000 types-croniter-2.0.0.20240423/croniter-stubs/croniter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/croniter-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:33.884474 types-croniter-2.0.0.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:33.884474 types-croniter-2.0.0.20240423/types_croniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/types_croniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/types_croniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/types_croniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 02:19:33.000000 types-croniter-2.0.0.20240423/types_croniter.egg-info/top_level.txt
```

### Comparing `types-croniter-2.0.0.20240321/CHANGELOG.md` & `types-croniter-2.0.0.20240423/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.0.0.20240423 (2024-04-23)
+
+croniter: add new `encoding` parameter to `is_valid` (#11808)
+
 ## 2.0.0.20240321 (2024-03-21)
 
 [croniter] Update to 2.0.3 (#11631)
 
 ## 2.0.0.20240318 (2024-03-18)
 
 Use `Final = ...` instead of `Final[Literal]` (#11623)
```

### Comparing `types-croniter-2.0.0.20240321/PKG-INFO` & `types-croniter-2.0.0.20240423/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 2.0.0.20240321
+Version: 2.0.0.20240423
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-croniter` aims to provide accurate annotations
 for `croniter==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5c75292f26aec8e6348a17d32077f408a1337988` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-croniter-2.0.0.20240321/croniter-stubs/croniter.pyi` & `types-croniter-2.0.0.20240423/croniter-stubs/croniter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def all_next(self, ret_type: _RetType | None = None) -> Iterator[Any]: ...
     def all_prev(self, ret_type: _RetType | None = None) -> Iterator[Any]: ...
     def iter(self, ret_type: _RetType | None = ...) -> Iterator[Any]: ...
     def is_leap(self, year: int) -> bool: ...
     @classmethod
     def expand(cls, expr_format: str, hash_id: bytes | None = None) -> tuple[list[list[str]], dict[str, set[int]]]: ...
     @classmethod
-    def is_valid(cls, expression: str, hash_id: bytes | None = None) -> bool: ...
+    def is_valid(cls, expression: str, hash_id: bytes | None = None, encoding: str = "UTF-8") -> bool: ...
     @classmethod
     def match(cls, cron_expression: str, testdate: float | datetime.datetime | None, day_or: bool = True) -> bool: ...
     @classmethod
     def match_range(
         cls, cron_expression: str, from_datetime: datetime.datetime, to_datetime: datetime.datetime, day_or: bool = True
     ) -> bool: ...
```

### Comparing `types-croniter-2.0.0.20240321/setup.py` & `types-croniter-2.0.0.20240423/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-croniter` aims to provide accurate annotations
 for `croniter==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5c75292f26aec8e6348a17d32077f408a1337988` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.20240321",
+      version="2.0.0.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['croniter-stubs'],
-      package_data={'croniter-stubs': ['__init__.pyi', 'croniter.pyi', 'METADATA.toml']},
+      package_data={'croniter-stubs': ['__init__.pyi', 'croniter.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-croniter-2.0.0.20240321/types_croniter.egg-info/PKG-INFO` & `types-croniter-2.0.0.20240423/types_croniter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 2.0.0.20240321
+Version: 2.0.0.20240423
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-croniter` aims to provide accurate annotations
 for `croniter==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5c75292f26aec8e6348a17d32077f408a1337988` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

